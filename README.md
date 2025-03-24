## Getting Started

First, run local redis server:

```bash
redis-server
```
Then, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```


最佳实践：Server Actions

定义在 actions 的代码要注意：
从 formData 中获取提交的数据
使用 zod 进行数据校验
使用 revalidate 更新数据缓存
返回合适的信息

定义表单的代码要注意：
搭配使用 useFormState 和 useFormStatus
特殊数据使用隐藏 input 提交
