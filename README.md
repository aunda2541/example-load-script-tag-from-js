Purpose of this repository is shows html parser wait until javacript file finished of coding lines but not wait data fetching.

Diagnose
1. You should get an error "Uncaught ReferenceError: $ is not defined" (because jquery not finished when html parsing ($("body").append($("<p>Hello, world</p>"));))
2. You can try to run ($("body").append($("<p>It works</p>"));) in your console.
3. "It works" appears on your web browser, that means jquery loaded perfectly.

-----------
4. try to uncomment  "<script src="./libs/jquery.js"></script>" in line 8
5. You won't get any error