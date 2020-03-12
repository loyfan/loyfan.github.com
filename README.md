## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/loyfan/loyfan.github.com/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

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
```go
package main

import "fmt"
import "time"

func main() {
	const INT32_MAX = int32(^uint32(0) >> 1)
	const INT64_MAX = int64(^uint64(0) >> 1)

	fmt.Print(INT32_MAX, INT64_MAX)
	fmt.Print("\n")
	
	const INT32_MIN = ^INT32_MAX
	const INT64_MIN = ^INT64_MAX

	fmt.Print(INT32_MIN, INT64_MIN)
	fmt.Print("\n")

	//fmt.Print(time.Unix(-int64(INT32_MAX)*9, 0))
	//fmt.Print(time.Unix(INT64_MIN/2-int64(INT32_MAX)*9, 0))

	fmt.Print(time.Unix(INT64_MIN+int64(INT32_MAX)*3, 0))
	fmt.Print("\n")
	fmt.Print(time.Unix(INT64_MAX, 0))
}
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/loyfan/loyfan.github.com/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
