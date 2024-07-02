# Problem 1
The JSON output from the AI pipeline needs to be parsed into a digestible format so that the front-end side can render detected rectangular bounding boxes and support additional graphical functionalities.
As an end user, a functionality for supporting focusing on the nearest bounding box is required. Below are additional requirements:
- Rectangles from AI output are given in “Location” format. Each location consists of xmin, ymin, xmax, ymax.
- Coordinates are based on imaginary coordinate axes, with the origin located at the top-left corner.
- Locations are given as an array of 4-number tuples: `[xmin, ymin, xmax, ymax]`
Implement the above requirements using the programming language of your choice, preferably Python if you can.


## Implementation requirements
The implementation should satisfy the following criteria:
- Leveraging OOP as much as it could.
- Convenience for both maintaining and extending the code base.
- Test-driven.


## Bonus
- Typing
- Modulizing
- Asynchronous programming
