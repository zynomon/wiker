---
layout: default
---

Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```


```mermaid
sequenceDiagram
    participant M as Main
    participant P as PluginLoader
    participant X as Xylem Plugin
    participant PH as Phloem Plugin
    participant S as Simple Plugin
    
    M->>P: loadAndInitialize()
    P->>P: Search plugin paths
    P->>P: Load .so/.dll/.dylib
    P->>P: Categorize by importance
    
    P->>X: initialize(window, settings, cmdLine)
    X-->>P: return true
    
    P->>PH: initialize(window, settings, cmdLine)
    PH-->>P: return true
    
    P->>S: initialize(window, settings, cmdLine)
    S-->>P: return true
    
    P->>P: Parse command line
    P-->>M: Initialization complete
    
    Note over M,S: Application runs
    
    M->>P: cleanup()
    P->>X: unload()
    P->>PH: unload()
    P->>S: unload()
```
 
---
 
### 1.4 Plugin vs Monolithic Design
 
```mermaid
graph LR
    subgraph Monolithic["Monolithic (Vex 1.x-3.x)"]
        A[Vex Application]
        A --> B[Editor]
        A --> C[Tabs]
        A --> D[Syntax]
        A --> E[Themes]
        A --> F[Everything]
    end
    
    subgraph Plugin["Plugin-Based (Vex 4.0+)"]
        G[Vex Core<br/>Minimal] --> H[VexCore.so]
        G --> I[SyntaxCore.so]
        G --> J[LookAndFeelCore.so]
        G --> K[Future.so]
    end
    
    style A fill:#8b0000,stroke:#ff0000,color:#fff
    style G fill:#006400,stroke:#00ff00,color:#fff
```
 
```mermaid
graph TD

A[Second instance] -->|writes your file arguments to| B[fileReq] --> |And second instance quits|C{First instance Reads it And opens that path in new tab} 

X[Third instance] -->|writes your file arguments to| Y[fileReq] --> |And Third instance quits|C

O[More instances works the same way]
```

```
The final element.
```