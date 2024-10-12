---
marp: true
paginate: true
footer: Here is the footer
theme: Chen
math: katex
---

`h1` can only be used once at the front page of the whole slide.

# MARP Theme Test

#### M1 Todai Taro

#### 1999/12/31

---

<!--_header: _header-->

## h2 and **h2 strong**

### This is h3

#### This is h4

##### This is h5 and h6

This is paragraph/text.

##### h5

**Lorem** ipsum **dolor** sit amet, consectetur adipisicing elit. Ipsam, quidem architecto animi quia **aliquid** odio aliquam asperiores sed **molestiae** labore repudiandae est sint iste cum impedit eaque blanditiis totam tempora.

- ##### Font size can be adjusted in `section --> font-size`

---

## **Code** & Code block

<!--_header: Code & Code block-->

##### You can write code blocks like this:

```python
# Additional information
EPOCH = 5
PATH = "model.pt"
LOSS = 0.4
torch.save({
            'epoch': EPOCH,
            'model_state_dict': net.state_dict(),
            'optimizer_state_dict': optimizer.state_dict(),
            'loss': LOSS,
            }, PATH)
```

```css
pre {
  display: block;
  margin: 1em 0 0 0;
  min-height: 1em;
  overflow: visible;
}
pre code {
  box-sizing: border-box;
  margin: 0em 0em;
  ...;
}
```

---

<!--_header: class="split-v"-->

## **Split** contents into multiple columns

##### Using the `split-v` class to divide content into columns

First, define `<div class="split-v">` , and then place 2, 3, or even more parallel `<div> ` blocks inside it.
You can define the width property for the nested `<div>` like this: `<div style="width: 25em;">`.
Here‘s an example:

<div class="split-v" style="margin-top:1.5em">

<div style="width:34em;border:2px solid #00000050;padding:0em 1em;border-radius:0.5em">

- ##### You can write a python code block like this:

```python
# Additional information
EPOCH = 5
PATH = "model.pt"
LOSS = 0.4
torch.save({
            'epoch': EPOCH,
            'model_state_dict': net.state_dict(),
            'optimizer_state_dict': optimizer.state_dict(),
            'loss': LOSS,
            }, PATH)
```

</div>
<div style="width:24em;border:2px solid #00000050;padding:0em 1em;border-radius:0.5em">

- ##### or a CSS code block like this:

```css
pre {
  display: block;
  margin: 1m 0 0 0;
  min-height: 1em;
  overflow: visible;
}
pre code {
  box-sizing: border-box;
  margin: 0em 0em;
  ...;
}
```

</div>

---

<!--_header: Margin & Padding of the "List"-->

## List

#### ul / ol / li

##### The spacing between all list items is controlled by the margin property in `ul > li {}`.

##### The margin property in `ul > li > p {}` controls the spacing between a list item and the previous list item..

- ##### This is a `ul` list. You can also include headings like this inside a list.

1. This is an `ol` list. The same properties apply as with `ul`.

   - ### h3 heading here
   - #### h4 heading here
   - Maintaining readability is important.

- I did't modify the margin property of `ul {}` .
- Some random text here.
- $E=mc^2$

---

<!--_header: Quote -->

## Quote

Some random content here

> Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem, blanditiis? Exercitationem harum libero ratione impedit soluta, dolores sit. Corporis illo, quaerat deserunt eligendi suscipit possimus facilis eveniet molestiae repellendus officia.</br>
> There can be some `codes` or **Bold texts** or $\text{KaTeX elements}$ inside a backquote block

Some random content here

---

<!--_header: Formula-->

## Formula

#### Math formula can be written in KaTeX:

##### Inline formulas

- Latent embedding space: $e \in R^{K\times D}$
- Embedding vectors in the codebook: $e_i \in R^D\quad i \in 1,2,\dots,K$

##### formula block

$$
f(x) = a_0 + \sum_{n=1}^{\infty} \left( a_n \cos\left(\frac{n \pi x}{L}\right) + b_n \sin\left(\frac{n \pi x}{L}\right) \right)
$$

---

## Table

| Table Head | No. | Column1 | Column2 |
| ---------- | --- | ------- | ------- |
|            | 1   | cat     | Anny    |
|            | 2   | dog     | Bane    |

##### You can also override the font-size of a table (remember to use 'em'):

<div style="font-size:1.5em">

| Table Head | No. | Column1 | Column2 |
| ---------- | --- | ------- | ------- |
|            | 1   | cat     | Anny    |
|            | 2   | dog     | Bane    |

</div>
