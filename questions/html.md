# HTML questions

<details>
  <summary>What were some of the key goals and motivations for the HTML5 specification?</summary>
  
  * encouraging semantic (meaningful) markup
  * rich content (graphics, movies, etc.) without the need for additional plugins, such as Flash
  * local storage in place of cookies
  * vector graphics using SVG and canvas
  * better cross-platform support whether running on a PC, Tablet, or Smartphone
</details>

<details>
  <summary>What parts of HTML have the greatest impact on SEO?</summary>
  
  * `<title>`
  * `<meta description="" content="">`
  * header tags: `h1, h2, h3`, etc.
  * image alt tags - search engines can read words
    ![searching by image alt tag](https://neilpatel.com/wp-content/uploads/2017/10/digital_marketing_-_Google_Search-1.png)
  * links and anchor tags text - Google looks to anchor text to understand what the link is about
</details>

<details>
  <summary>What are <code>data-*</code> attributes good for?</summary>
  
  * `data-*` attributes allows us to store extra information on standard, semantic elements
    ```html
    <div data-example="100">Example</div>
    ```
  * access in JavaScript:
    ```js
    const div = document.querySelector('div');

    // Get value
    div.dataset.example;
    // Set value
    div.dataset.example = 999;
    ```
  * access in CSS
    ```css
    div::after {
      content: attr(data-example);
    }
    ```
</details>
