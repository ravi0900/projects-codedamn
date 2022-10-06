In this step you have to make sure that the nav bar is dynamically fix while scolling text animation is working properly.



The following are the code exmaple to use in index.js file for nav fix and text animation : 

```nav bar position
const navBar = document.querySelector(".nav");
const navHeight = navBar.getBoundingClientRect().height;
window.addEventListener("scroll", () => {
  const scrollHeight = window.pageYOffset;
  if (scrollHeight > navHeight) {
    navBar.classList.add("fix-nav");
  } else {
    navBar.classList.remove("fix-nav");
  }
});
```


```text animation  
new TypeIt("#type1", {
  speed: 120,
  loop: true,
  waitUntilVisible: true,
})
  .type("Dev", { delay: 400 })
  .pause(500)
  .delete(9)
  .go();
```



You can adjust the scroll speed and animation. 

