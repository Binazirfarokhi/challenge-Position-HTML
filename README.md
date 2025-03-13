# challenge-Position-HTML

Types of Positioning
1. position: relative;
Makes an element positioned (so it can now respond to top, bottom, left, and right).
Keeps the element in the document flow (other elements still respect its space).
Moves the element relative to its original position.
The main challenge is that the original space remains in the document, even if the element is moved.
2. position: absolute;
Removes the element from the normal document flow (other elements ignore its space).
The element is positioned relative to its closest positioned ancestor (relative, absolute, or fixed).
If no such ancestor exists, it is positioned relative to the <html> (viewport).
It does not affect sibling elements because it's taken out of the document flow.
Important Note:
"position: absolute; works with position: relative;" → Not always!
It actually positions itself relative to the nearest ancestor that has relative, absolute, or fixed positioning.

3. position: fixed;
Works like absolute, but ignores parent elements entirely.
Always positions itself relative to the viewport (browser window).
Stays fixed in place even when scrolling.
4. position: sticky;
Hybrid of relative and fixed positioning.
Acts as relative until a certain scroll position is reached, then it becomes fixed.
Requires scrolling content to work—if there's no scrolling, sticky won't take effect.