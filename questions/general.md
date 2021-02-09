# General questions

<details>
  <summary>What excites or interests you about coding?</summary>
  
  * the only limitation is our imagination
  * solving problems and building apps that make our lives easier
  * learning something new everyday
</details>

<details>
  <summary>What is CDN?</summary>
  
  * Content Delivery Network
  * services that allow us to use libraries, frameworks, etc. without the need to actually attach additional files
    to our project.
  * all we have to do is attach a script from cdn:
  ```javascript
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.6/umd/popper.min.js"></script>
  ```
  * benefits:
    * faster delivery of content - because CDN is a geographically distributed network, if our website is based in the UK and we get traffic from the U.S., it’s possible that your CDN provider has a server in the U.S. and will use that server for your website.
    * more simultaneous users - large number of users can access the network at the same time without delays
    * our project bundles is lighter so we don't clutter the server disk space
  * disadvantages:
    * CDN can fail to
    * we don't know how long the services will be supported
    * restrictions, some countries have blocked the domains or IP addresses of popular CDNs
</details>

<details>
  <summary>What does DRY stands for?</summary>
  
  * Don't Repeat Yourself
  * one of the Clean Code principles
  * we should try not to repeat ourselves in the code
  * if there is a lot of repetitions in our code it:
    * is harder to read
    * becomes suboptimal
    * is harder to maintain and slow us down - in case of a bug we have to fix it in many places
</details>

<details>
  <summary>What is npm?</summary>
  
  * node package manager
    * an online repository that hosts JavaScript packages
    * a CLI (command-line interface) for publishing and downloading packages
</details>





