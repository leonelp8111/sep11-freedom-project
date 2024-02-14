# Entry 3
##### 2/11/24

### Now during learning kaboom.js I am trying to add a health system to the game that I have made to demo how some of the functions work. However I'm still having some trouble with having the health system work. For the things that I have been trying to add were as i said before was a health system because right now in my game. Currently in my game the player can only jump and avoid obstacles. I made it so that the player can only jump after hitting the floor with this line of code.
 ```
 onKeyPress("space" , () => {
    if (spider.isGrounded()) {
    spider.jump()
    }
})
```
### Spider is the name I gave the sprite so what the code is saying is when the key "space" is pressed if the player:Spider is touching the ground allow them to jump. This makes sure that they can't spam the jump button and avoid all the obstacles entirely. But without an actual stop or danger to the game it makes it endless. I also plan to add a way to score how long the playter can stay alive. But back to the health function, which I'm still figuring out myself. I have the right code and even tested it out.
```
spider.onCollide("tree" , "bad ", () => {
    addKaboom(spider.pos);
    shake();
    spider.hurt(1)
    bad.hurt(1)
});
```
### What this code is saying is that when the player touches or collides with any of the tress then it will categorize as bad and it will display a kaboom effect from where the players postiton is. Now this is where I'm stuck, when creating the player you also add how much health you would want they to have. To see if anything would happen I put the players health to one and at the bottom of the code snippet displayed above it says that it should deal one of damage of the players health. But it only worked partially as right after getting hit the game would go blank and you woud have to resart the page to play again. I was stuck on what was happening until I asked the person next to me if he had a similar problem. Luis told me that I had to add a screen that plays once the player has died. He also told me to look back at the documentation on the [kaboom](https://kaboomjs.com/) documentatio. For my engineering design process I am planning the most promising soultions since I'm trying to learn how to use the health which going to be a big part of my main project. For the next part of my project I want to learn how to make enimies in the game that don't just stay in one place that the player has to avoid. I took a peek at how it would be done and I think all I have to do is make another sprite that isnt controlled and comes after the player but I have yet to figure out the other parts. 

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)