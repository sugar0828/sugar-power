## Welcome to GitHub Pages

## vite 个人使用遇到的问题和解法的记录

### 对依赖预构建的理解
最初不理解预构建和打包的区别，所以当看到使用Rollup来打包，又看到还有Esbuild时候，心生疑惑：二者为何同时出现，只有一个不够了吗？同时出现，那二者的各种作用是什么？
以下是后来的理解：
1. 首先说下他们各自的作用：ESbuild作用体现在本地开发阶段；Rollup作用是在生产环境上，也就是发布到线上环境时候。
2. ESbuild是用来在dev阶段做预构建的，预构建有2个目的
  1. CommonJS 和 UMD 兼容性: 开发阶段中，Vite 的开发服务器将所有代码视为原生 ES 模块。因此，Vite 必须先将作为 CommonJS 或 UMD 发布的依赖项转换为 ESM。
  2. 性能： Vite 将有许多内部模块的 ESM 依赖关系转换为单个模块，以提高后续页面加载性能。参考官网的举例说明：https://cn.vitejs.dev/guide/dep-pre-bundling.html#the-why

### 

You can use the [editor on GitHub](https://github.com/sugar0828/sugar-power.github.io/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/sugar0828/sugar-power.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
