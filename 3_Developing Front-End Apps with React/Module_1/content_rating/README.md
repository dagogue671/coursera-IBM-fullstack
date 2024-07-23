# coding-project-template

## Notes from Learner

Running **npm run preview** fails to run.
Running **npm run dev** works.

The alternative to run this is to edit the **package.json** file in the root folder and change the script configs. Important part is to change the **"preview": "vite build; vite preview --help"**. to **"preview": "vite preview"**.

Then run **npm run build** then **npm run preview** to make it work.

```
"scripts": {
    "dev": "vite",
    "build": "vite build",
    "lint": "eslint . --ext js,jsx --report-unused-disable-directives --max-warnings 0",
    "preview": "vite preview"
  },
```
