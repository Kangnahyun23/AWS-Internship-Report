---
title: "Chuẩn bị môi trường phát triển"
weight: 1
chapter: false
pre: " <b> 5.1. </b> "
---

### 1. Cài đặt công cụ (Prerequisites)

Để phát triển ứng dụng web hiện đại, bạn cần chuẩn bị các công cụ tiêu chuẩn sau:

*   **Node.js (LTS Version):** Môi trường runtime cho JavaScript/TypeScript.
*   **Git:** Hệ thống quản lý phiên bản phân tán.
*   **IDE:** Visual Studio Code (khuyên dùng).

**VS Code Extensions khuyến nghị:**
*   **ESLint & Prettier:** Tự động format và kiểm tra lỗi code.
*   **Tailwind CSS IntelliSense:** Gợi ý class Tailwind cực nhanh.
*   **ES7+ React/Redux/React-Native snippets:** Code nhanh hơn với các phím tắt.

### 2. Khởi tạo dự án Next.js

Chúng ta sẽ sử dụng **Next.js** - React Framework phổ biến nhất hiện nay.

Chạy lệnh khởi tạo:

```bash
npx create-next-app@latest my-serverless-app
```

Cấu hình chi tiết:
*   TypeScript: **Yes** (Tăng tính chặt chẽ cho code)
*   Tailwind CSS: **Yes** (Styling nhanh chóng)
*   ESLint: **Yes** (Kiểm tra lỗi)
*   App Router: **Yes** (Kiến trúc routing mới nhất)
*   Import Alias: **@/** (Giúp import file gọn gàng hơn)

### 3. Cấu trúc dự án chuẩn (Project Structure)

Một cấu trúc thư mục khoa học giúp dự án dễ bảo trì về sau:

![VS Code Project Structure](/images/vscode_project_structure_1764663000000.png)

*   `src/app`: Chứa các Pages và Layout (App Router).
*   `src/components`: Chứa các UI Components tái sử dụng (Button, Card...).
*   `src/hooks`: Chứa Custom Hooks (useAuth, useChat...).
*   `src/lib`: Chứa các hàm tiện ích (utils) và cấu hình (AWS config).

### 4. Cấu hình `tsconfig.json` (Best Practices)

Để đảm bảo code TypeScript chặt chẽ nhất, hãy cập nhật `tsconfig.json`:

```json
{
  "compilerOptions": {
    "target": "es5",
    "lib": ["dom", "dom.iterable", "esnext"],
    "allowJs": true,
    "skipLibCheck": true,
    "strict": true, // Quan trọng: Bật chế độ nghiêm ngặt
    "forceConsistentCasingInFileNames": true,
    "noEmit": true,
    "esModuleInterop": true,
    "module": "esnext",
    "moduleResolution": "node",
    "resolveJsonModule": true,
    "isolatedModules": true,
    "jsx": "preserve",
    "incremental": true,
    "plugins": [
      {
        "name": "next"
      }
    ],
    "paths": {
      "@/*": ["./src/*"]
    }
  },
  "include": ["next-env.d.ts", "**/*.ts", "**/*.tsx", ".next/types/**/*.ts"],
  "exclude": ["node_modules"]
}
```

### 5. Cài đặt thư viện UI bổ trợ

```bash
cd my-serverless-app
npm install framer-motion lucide-react clsx tailwind-merge
```

### 6. Cấu hình TailwindCSS

Thiết lập các biến màu (CSS Variables) trong `tailwind.config.ts` để đảm bảo tính nhất quán về thiết kế (Design System).

```typescript
// tailwind.config.ts
import type { Config } from "tailwindcss";

const config: Config = {
  content: [
    "./src/pages/**/*.{js,ts,jsx,tsx,mdx}",
    "./src/components/**/*.{js,ts,jsx,tsx,mdx}",
    "./src/app/**/*.{js,ts,jsx,tsx,mdx}",
  ],
  theme: {
    extend: {
      colors: {
        primary: "#432c7a", // Màu chủ đạo
        secondary: "#764ba2",
        accent: "#ffd700",
        background: "#1a0b2e", // Màu nền tối
      },
      backgroundImage: {
        "gradient-radial": "radial-gradient(var(--tw-gradient-stops))",
      },
    },
  },
  plugins: [],
};
export default config;
```

---

### Chuyện nghề (My Experience)

{{% notice note %}}
**Tại sao lại là TypeScript?**
Hồi mới làm quen, mình thấy TypeScript khá phiền phức vì cứ báo lỗi đỏ lòm. Nhưng khi dự án phình to lên, chính những dòng báo lỗi đó đã cứu mình khỏi hàng tá bug ngớ ngẩn (như gõ sai tên biến, truyền sai kiểu dữ liệu).
**Lời khuyên:** Hãy bật `strict: true` ngay từ đầu. "Khổ trước sướng sau"!
{{% /notice %}}

### Kiểm thử & Xác thực (Verification)

Để đảm bảo môi trường đã sẵn sàng, hãy thực hiện các bước kiểm tra sau:

**Test Case 1: Kiểm tra phiên bản Node.js**
Mở terminal và chạy:
```bash
node -v
```
*Kết quả mong đợi:* `v18.x.x` hoặc cao hơn (LTS).

**Test Case 2: Chạy thử server**
```bash
npm run dev
```
*Kết quả mong đợi:* Terminal hiển thị:
```
ready - started server on 0.0.0.0:3000, url: http://localhost:3000
event - compiled client and server successfully in 1234 ms (150 modules)
```
Truy cập trình duyệt thấy logo Next.js xoay vòng là thành công!
