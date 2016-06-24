# Hands-on Demo with Construct 2

### 1. Adding Player
- After creating a new project go to your first layout, right click anywhere on the screen and click 'Insert new object'
- From the popup, select 'sprite,' name it 'player,' then click 'done.'
- The popup will disappear and to add your new sprite, left click anywhere on the screen.
- A popup will appear allowing you to edit the way your player looks. Give it a solid colour for now (you can change it later).
- Close the popup windows and go to the property panel (located to the left of your screen) and change the size of your player to ```50, 50```.


### 2. Adding Enemies 
- Repeat step 1 but this time give your enemy sprite a different colour from that of your player sprite.
- Right click on your enemy sprite, click 'copy,' then right click anywhere on your layout and click 'paste' to create a duplicate of your enemy sprite. Do that a couple more times.


### 3. Adding Controls to your Player Sprite
- Click on your player sprite so that it's selected and go to the property panel.
- Under 'edit/behaviours' click 'behaviours'.
- From the popup window click on the '+' icon and add the '8 Direction' and 'Scroll To' behaviour.
- Close the popup windows when you're done.


### 4. Adding Events
- Now navigate to your event sheet for the layout you've been working on.
- Add a new event.
- Click on your player sprite and what you want is 'On collision with another object'.
- Click 'next' and select your enemy sprite from the drop down. Click 'done' when you're ready.


### 5. Adding Action
- Now that you have an event lets add make it do something! Click 'Add actions' and from the popup window click on your enemy sprite, click 'next' and select 'Destroy'.
- Click 'Add actions' again and this time select 'System'. Click 'next' and this time select 'Create object'. Click 'next' and from the dropdown menu select your enemy sprite. For layer leave it as 0. For x what we want to do is randomly place our new enemy sprite somewhere on the screen. The way to do that is with ```random(LayoutWidth)```. What this does is it's grabbing the width of our layout and then randomly picking a number between 0 and the whatever the layout width is. For y use ```random(LayoutHeight)```.
- Now we'll increase the size of our player. To do that add another action but this time select our player sprite again. Click 'next' and what we want to do is select 'Set size'. Click 'next' and for width and height what we want to do is get the player's current width and height (whatever it may be) and add some amount to it so each time when we collide with an enemy our overall size keeps increasing. So to do that, for width, use ```Self.Width+5``` and for height, use ```Self.Height+5```.


### 6. Add Scoring
- Go back to your layout and on the right hand side of your screen you should see a tab called 'Layer'. Click on it and add a new layer. Call it HUD if you like.
- With that newly added layer selected, in the property panel, make sure 'Parallax' is set to ```0, 0```.
- Just like with step 1, right click on your layout and click 'Insert new object'. This time we want to select the text object. Name it score then click 'done'.
- Add it to the top left had corner of your layout.
- From the property window make sure 'Layer' is set to your newly added layer.

### 7. Global Variable
- Go back to your event sheet and now right click and click 'Add global variable'.
- Make sure it's set to 'number', the initial value is 0 and name it 'Score'. This will be used to keep track of the player's current score.

### 8. Increasing Score
- Now add another action under your first event. Click 'System' and click 'Add to Global Variable'.
- Increase by 1.
- Add another action but this time selecting your text object score. You want to then click 'Set text' and enter the name of your global variable. Should be 'Score'.

And now you're done!