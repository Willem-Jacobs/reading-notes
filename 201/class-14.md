# Class 14 Reading

[Return to 201 TOC](201TOC.md)

*Resource: <https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html>

## What Google learned on its quest to build the perfect team

- That understanding and influencing group norms were the keys to improving teams.
- The norms of one team sometimes contrasted sharply with those of another team.
- Data of the norms was not clear and sometimes pointed in opposite directions.
- The norm of a team could make the team always fail or always succeed compared to others regardless of the ability level of the team members.
- Open discussion seams to be one norm where each member has equal speaking time, the team did well.
- Average social sensitivity seems to be a strong norm for a team to have collectively.
- Psycological safety is another strong norm. This being internersonal trust and mutual respect in which people are comfortable being themeselves.
- For Google the data indicated that psycological safety, more than anything else, was ciritical to making a team work.
- Google had to find a way to make communication and empathy the building blocks of forging real connections for teams.
- "The behaviors that create psychological safety — conversational turn-taking and empathy — are part of the same unwritten rules we often turn to, as individuals, when we need to establish a bond. And those human bonds matter as much at work as anywhere else. In fact, they sometimes matter more." * Quote from the article.
- "No one wants to leave part of their personality and inner life at home. But to be fully present at work, to feel ‘‘psychologically safe,’’ we must know that we can be free enough, sometimes, to share the things that scare us without fear of recriminations. We must be able to talk about what is messy or sad, to have hard conversations with colleagues who are driving us crazy. We can’t be focused just on efficiency. Rather, when we start the morning by collaborating with a team of engineers and then send emails to our marketing colleagues and then jump on a conference call, we want to know that those people really hear us. We want to know that work is more than just labor." * Quote from the artile.
- In the best teams, members listen to one another and show sensitivity to feelings and needs.

*Resource: <https://learn.shayhowe.com/advanced-html-css/css-transforms/>

## CSS Transforms

- Transform CSS property has 2 settings for 2D and 3D and each of these has its own individual properties.
- 2D works on the X and Y axis while 3D adds the Z axis.
- Property `rotate` allows the rotation of an item in degrees. Positive values for clockwise and negative values for counter-clockwise.
- Property `scale` allows the change of the size of the element. Decimal numbers makes the item smaller and numbers above one make it larger. You can use `scaleX or scaleY` to change only that dimension of the element.
- Property `translate` works a bit like the relative positioning by pushing or pulling an element in different directions. `translateX or translateY` can be used seperate or combined where x is first seperated by a comma then the y value. General length like pixel, em, rem or percentage. Positive numbers push down and to right while negative numbers pull up and to the left of its original position.
- Property `skew` is used to distort elements on the horizontal axis, vertical axis, or both. This has a `skewX or skewY` that can be seperated or combined like the others with `(x, y)` as values of degrees.
- These properties can all be combined into 1 line seperated by a space.
- The default transform origin is the dead center of the element but this can be changed by using the `transform-origin` property. This property can take pixel or percentage or words like top left, bottom right. If only 1 value is specified it is applied to the x & y axis or you specify 2 values.
- Property `perspective` can be used to make objects have depth. This can be used along with the transform property on an element or set directy on the parent element containing the elements. Using it with transform is good for a single element on its own perspective. Using it on a group is good for all items based on the overall perspective of their layout on the screen. Perspective takes a value in length or the word none. When using none, no perspective is set and using a value will make the item look further away at the far away point. Higher the number further away.
- Perspective also has an origin point called `perspective-origin` that works the same and the `transform-origin` but this determines the vanishing point of a transform.
- 3D has properties to rotate item on each axis `rotateX, rotateY, rotateZ` these work the same as the normal rotate but just on each independant axis.
- 3D can be scaled on the `scaleZ` property same as the normal 2D scale.
- 3D can be translated using the `translateZ` property same as the normal 2D translate.
- 3D has a `backface-visibility` property that takes hidden or visible values. This to determine if the element content will be seen when rotated 180 degrees or not.

*Resource: <https://learn.shayhowe.com/advanced-html-css/transitions-animations/>

## CSS Transition & Animation

- For transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using :hover, :focus, :active and :target psuedo-classes.
- There are 4 transition related properties `transition-property, transition-duration, transition-timing-function, transition-delay` with the first 3 being the most popular and not all need to be used.
- Transition-property is used to specify which property will be altered with the transition settings specified. Multiple properties can be set seperated by a comma and you can also say all to impact all properties.
- Only properties that have a identifiable halfway point can be used for transition.
- Transition-duration is a value in s or ms (seconds or milliseconds) to control the speed of the transition. Multiple values can be set seperated by command and each value is for the property set in the transition property when you have multiple properites set.
- Transition-timing-function is used to set the transition type being `linear, ease-in, ease-out, ease-in-out`. Linear is a constant speed. Ease-in starts slow and speeds up. Ease-out starts fast and slows down. Ease-in-out starts slow, speeds up in middle, slows down going back out.
- Transition-delay is used to set a time in seconds or milliseconds that the transition should wait before starting.

[Return to 201 TOC](201TOC.md)

[Return to Main Page](../README.md)
