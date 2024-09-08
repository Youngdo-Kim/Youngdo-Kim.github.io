---
layout: post
title: Comprehensive Particulate Matter (PM) Studies Using DIHM
truncated_preview: true
excerpt_separator: <!--more-->
---

<div class="message">
  환경오염이 심해지면서 particulate matter에 대한 관심과 연구가 점점 커지고 있다. 여기에서는 DIHM을 이용해서 식물에 settling하는 PM의 dynamics를 연구하고 물에 떠다니는 PM의 농도를 측정하는 방법을 개발하였다. 여기서는 공저자로서 실험 셋업 개발이나 formal analysis에 기여하며 DIHM 기술 습득과 AI model을 익히는 유용한 기회였다.
</div>

## Visualizing Faster PM Deposition on Trichome-Rich Plant Leaves

Published as a co-author, Journal of Environmental Management (2023/04)
<br> 나뭇잎 연구에서는 PM이 식물 가까이에 접근하면서 식물의 Trichome에 접근하면 점점 빨라지는 속도장을 DIHM으로 가시화했다. 가시화 결과 Trichome에 접근할 수록 뾰족한 trichome에 의해 강화된 전기장 때문에 PM의 속도가 점점 빨라짐을 알 수 있다.

<div class="container">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf1.jpg" alt="Perilla leaf" style="width: 200px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">1. Experimental setup</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf3.gif" alt="Acquired images" style="width: 200px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">2. Acquired PM images</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf2.jpeg" alt="Velocity visualization" style="width: 200px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">3. Velocity field visulization</figcaption>
  </figure>
</div>

나는 leaf위에 낙하하는 PM settling velocity의 reference가 되는 freely falling PM의 velocity를 구했다. PM은 drag와 gravitational force가 평형을 이루며,
그 공식은 $$V_{s,\text{theor}} = \frac{C_C (\rho_{PM} - \rho_{air}) g D^2}{18 k_s / \mu_{air}}$$ 이다. Through this project, I gained experience in optical setup, imaging, reconstruction, and particle tracking using DIHM.
<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/Leaf4.jpg" alt="Velocity distribution" style="width: auto; height: auto; display: block; margin: 0 auto;">
  <figcaption style="font-size: 0.9em; color: #555;">4. Settling velocity graph by PM diameter</figcaption>
</figure>
<br><b>Publication:</b> Kim, J., Kim, J., <b>Kim, Y.</b>, Go, T., and Lee, S. J. (2023). Accelerated settling velocity of airborne particulate matter on hairy plant leaves. J. Environ. Manage. 332, 117313. doi:10.1016/j.jenvman.2023.117313


## Smartphone-based holographic measurement of polydisperse suspended particulate matter with various mass concentration ratios

Published as a co-author, Scientific Reports (2022/12)
<br>
<div class="container">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/smart1.jpeg" alt="Velocity distribution" style="width: auto; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">1. Principle of speckle pattern generation</figcaption>
    </figure>
    <div class="text">
        <h2>
          Title
        </h2>
        <p>
          The second project aimed to replace expensive conventional particulate matter (PM) measuring devices with a smartphone-based solution. Using DIHM and artificial intelligence,
          we predicted the PM concentration in a solution containing a mixture of fine PM (approximately 1.2 micrometers) and coarse PM (7.6 micrometers).
          I was responsible for the optical setup and sample preparation. We were able to create the setup for under $400 using a 3D printer and a Samsung smartphone.
          An object produces fringe patterns, and when these fringe patterns accumulate, they form a speckle pattern.
        </p>
    </div>
</div>


<div class="container">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart2.png" alt="Experimental setup" style="width: 200px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">2. Experimental setup</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart3.png" alt="Fine PM concentration prediction" style="width: 200px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">3. Fine PM concentration prediction</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart4.png" alt="Coarse PM concentration prediction" style="width: 200px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">4. Coarse PM concentration prediction</figcaption>
  </figure>
</div>

<br><b>Publication:</b> Kim, J., <b>Kim, Y.</b>, Howard, K. J. and Lee, S. J. (2022). Smartphone-based holographic measurement of polydisperse suspended particulate matter with various mass concentration ratios. Sci. Rep. 12, 22609. https://doi.org/10.1038/s41598-022-27215-6

<!--
- **To bold text**, use `<strong>`.
- *To italicize text*, use `<em>`.
- Abbreviations, like <abbr title="HyperText Markup Langage">HTML</abbr> should use `<abbr>`, with an optional `title` attribute for the full phrase.
- Citations, like <cite>&mdash; Mark otto</cite>, should use `<cite>`.
- <del>Deleted</del> text should use `<del>` and <ins>inserted</ins> text should use `<ins>`.
- Superscript <sup>text</sup> uses `<sup>` and subscript <sub>text</sub> uses `<sub>`.

Most of these elements are styled by browsers with few modifications on our part.

## Truncated Post Previews

Celeste also supports truncated post previews that are customizable on a per-post basis. This is a sample of how a truncated post looks like. Click on **Read more** to see the rest of the post!

<!--more-->

More details on how to use truncated post previews are in the [v1.4.0 release notes](https://github.com/nicoelayda/celeste/releases/tag/v1.4.0).

-----

Cum sociis natoque penatibus et magnis <a href="#">dis parturient montes</a>, nascetur ridiculus mus. *Aenean eu leo quam.* Pellentesque ornare sem lacinia quam venenatis vestibulum. Sed posuere consectetur est at lobortis. Cras mattis consectetur purus sit amet fermentum.

> Curabitur blandit tempus porttitor. Nullam quis risus eget urna mollis ornare vel eu leo. Nullam id dolor id nibh ultricies vehicula ut id elit.

Etiam porta **sem malesuada magna** mollis euismod. Cras mattis consectetur purus sit amet fermentum. Aenean lacinia bibendum nulla sed consectetur.

## Footnotes

Footnotes are supported as part of the Markdown syntax. Here's one in action. Clicking this number[^fn-sample_footnote] will lead you to a footnote. The syntax looks like:

{% highlight text %}
Clicking this number[^fn-sample_footnote]
{% endhighlight %}

Each footnote needs the `^fn-` prefix and a unique ID to be referenced for the footnoted content. The syntax for that list looks something like this:

{% highlight text %}
[^fn-sample_footnote]: Handy! Now click the return link to go back.
{% endhighlight %}

You can place the footnoted content wherever you like. Markdown parsers should properly place it at the bottom of the post.

## Heading

Vivamus sagittis lacus vel augue rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros.

### Code

Inline code is available with the `<code>` element. Snippets of multiple lines of code are supported through [rouge](https://github.com/jneen/rouge). Longer lines will automatically scroll horizontally when needed.

{% highlight js %}
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
{% endhighlight %}

You may also optionally show code snippets with line numbers. Add `linenos` to the rouge tags.

{% highlight js linenos %}
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
{% endhighlight %}

Aenean lacinia bibendum nulla sed consectetur. Etiam porta sem malesuada magna mollis euismod. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa.

### Gists via GitHub Pages

Vestibulum id ligula porta felis euismod semper. Nullam quis risus eget urna mollis ornare vel eu leo. Donec sed odio dui.

{% gist 13f94b734a4ddb132735 gist.md %}

Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Nullam quis risus eget urna mollis ornare vel eu leo. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec sed odio dui. Vestibulum id ligula porta felis euismod semper.

### Lists

Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Aenean lacinia bibendum nulla sed consectetur. Etiam porta sem malesuada magna mollis euismod. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.

* Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
* Donec id elit non mi porta gravida at eget metus.
* Nulla vitae elit libero, a pharetra augue.

Donec ullamcorper nulla non metus auctor fringilla. Nulla vitae elit libero, a pharetra augue.

1. Vestibulum id ligula porta felis euismod semper.
2. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
3. Maecenas sed diam eget risus varius blandit sit amet non magna.

Cras mattis consectetur purus sit amet fermentum. Sed posuere consectetur est at lobortis.

<dl>
  <dt>HyperText Markup Language (HTML)</dt>
  <dd>The language used to describe and define the content of a Web page</dd>

  <dt>Cascading Style Sheets (CSS)</dt>
  <dd>Used to describe the appearance of Web content</dd>

  <dt>JavaScript (JS)</dt>
  <dd>The programming language used to build advanced Web sites and applications</dd>
</dl>

Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Nullam quis risus eget urna mollis ornare vel eu leo.

### Images

Quisque consequat sapien eget quam rhoncus, sit amet laoreet diam tempus. Aliquam aliquam metus erat, a pulvinar turpis suscipit at.

![placeholder](http://placehold.it/800x400 "Large example image")
![placeholder](http://placehold.it/400x200 "Medium example image")
![placeholder](http://placehold.it/200x200 "Small example image")

### Tables

Aenean lacinia bibendum nulla sed consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Upvotes</th>
      <th>Downvotes</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td>Totals</td>
      <td>21</td>
      <td>23</td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>10</td>
      <td>11</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <td>Charlie</td>
      <td>7</td>
      <td>9</td>
    </tr>
  </tbody>
</table>

Nullam id dolor id nibh ultricies vehicula ut id elit. Sed posuere consectetur est at lobortis. Nullam quis risus eget urna mollis ornare vel eu leo.

-----

Want to see something else added? <a href="https://github.com/nicoelayda/celeste/issues/new">Open an issue.</a>

[^fn-sample_footnote]: Handy! Now click the return link to go back.
-->
