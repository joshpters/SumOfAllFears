# Sum Of All Fears Minisite

This is a complete minisite that contains a visual representation of the "Sum Of All Fears" challenge.

![Screenshot](/Images/screenshot.jpg)

This project was created using Bootstrap 4.5, HTML5, CSS3, and JavaScript. All logic & JavaScript DOM changes were custom coded for this project.

## What is the "Sum Of All Fears" challenge?

Given a list of numbers and a number K, return whether any two numbers from the list add up to K.

This challenge or a slight variation has been used by technology companies such as
Amazon and Google and was also featured as a Daily Coding Problem in dev.to.

## Installation

You can view this site [live](https://sumofallfears-challenge.netlify.app/).

To download and run locally, clone this repository and open index.html.

``` sourceCode
git clone https://github.com/joshpters/SumOfAllFears
```

## Core Functions

I have built two variations, one that finds all pairs and on that just determines if there is a pair of numbers that add up to K.

The minisite has a modified version of function A to work with the page animations & DOM changes.

```javascript
//function that finds all matches
function sumOfAllFearsA(fears, k) {
    matches = [];
    for (r = 0; r < fears.length; r++) {
        for (i = r + 1; i < fears.length; i++) {
            if (fears[r] + fears[i] == k) {
                matches.push([fears[r], fears[i]])
            }
        }
    }
    return matches;
}

//function that returns true or false
function sumOfAllFearsB(fears, k) {
    for (r = 0; r < fears.length; r++) {
        for (i = r + 1; i < fears.length; i++) {
            if (fears[r] + fears[i] == k) {
                return true;
            }
        }
    }
    return false;
}
```


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.