# Classify

So now you've got some basic divisions (or `<div>`s) of the different parts of
notification component, let's start to specify our elements beyond just `<div>`.

In our page example, there are a lot more elements to work with, but the
principles should still carry over. The thing you want to look for is places you
can replace `<div>`s with other more semantic elements.

> Side note: "Semantic" in the context of HTML usually means that the element in
> use describes what the element is used for. For example, a `<nav>` element
> describes navigation, and `<main>` describes the main content. `<div>` isn't
> very semantic beyond just saying that it is an element, or box containing
> other elements. `<div>`s are useful for layout and dividing different elements
> from one another, but it is generally better to give meaning where you can.

Regardless of whether or not we can classify and element with it's HTML tag,
it's a good idea to add classes to elements we can otherwise not specify. This
will help us style thing and lay things out. Also try to reuse classes when you
have elements that should be styled similarly. Usually this is apparent when you
have a repeating list of items. If there are items that are mostly the same with
something only slightly different, you can apply a secondary class to the items
that are slightly different.

Below is the previous example with various HTML tags and classes.

```html
<div class="page-wrapper">
  <header class="page-header">
    <img class="logo" />
    <nav class="page-navigation">
      <!-- We added a `ul` here since we have "list" of sorts -->
      <ul>
        <li>
          <span>Products</span>
          <img class="product-icon" />
        </li>
        <li>
          <span>Use Cases</span>
          <img class="product-icon" />
        </li>
        <li>
          <span>Developers</span>
        </li>
        <li>
          <span>Pricing</span>
        </li>
      </ul>
    </nav>
    <button class="free-trial">Try Free</button>
  </header>
  <main class="main-content">
    <div class="left-section">
      <h2 class="headline">Reach your audience instantly &amp; exclusively</h2>
      <h3 class="details">
        Our services pack a serious punch, from award winning web design and
        social media marketing to your startup
      </h3>
      <div class="actions">
        <button class="call-to-action">Get Started</button>
        <button class="call-to-action borderless">
          <img class="video-icon" />
          <span>Watch Video</span>
        </button>
      </div>
      <button class="button-icon"></button>
    </div>
    <div class="right-section">
      <img class="hero-image" />
    </div>
  </main>
  <footer class="page-footer">
    <ul class="feature-list">
      <li class="feature-box">
        <span>
          Our powerful campaigns will get your brand front and center on major
          networks
        </span>
        <img class="feature-icon" />
      </li>
      <li class="feature-box">
        <span>
          We offer a beautiful, high end website that hooks your potential
          audiences.
        </span>
        <img class="feature-icon" />
      </li>
      <li class="feature-box">
        <span>
          Our expert design team will craft your Startup identity from the
          ground up.
        </span>
        <img class="feature-icon" />
      </li>
    </ul>
  </footer>
</div>
```

Now apply this to your notifications component. You may not have as diverse a
set of HTML tags to use, but classes will help here.

Once you've put in the classes and adjusted the HTML tags to your liking, move
on to the [next exercise](./04_notifications_layout.md)
