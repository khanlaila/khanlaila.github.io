# Homework 2 - CSCI 39548
# Name: Laila Khan

## 1. Explain the difference between flex-direction: row and flex-direction: column.
flex-direction: row places flex items side by side horizontally, which is the default. I used this for my navigation bar so that my logo sits on the left and my nav links sit to the right. All in one horizontal line.
flex-direction: column stacks flex items side by side vertically, one on top of the other. This was used in my media query to make the navbar and its links collapse downward on mobile, so each link can get its own row instead of being together.

## 2. Why is it important to use relative units (like %, vh, or rem) instead of fixed pixels (px) for responsive design?
Fixed pixel values do not adapt to different screen sizes. For example, if I set something to 'width: 900px', it would overflow on a small phone screen. The % unit adjusts based on the parents element's size, so a 'width: 100%' card always fills its container whether on a small phone or wide monitor etc. Using relative units means I'm able to write less code and the layout adapts to any device.

## 3. AI Attribution
Prompt Used: "Write a media query so my navbar links stack vertically on mobile and the height adjusts"

provided code:
@media (max-width: 768px) {
  .navbar { flex-direction: column; }
  .nav-links { flex-direction: column; }
}
I had to modify my height because it did not account for fixed height. 