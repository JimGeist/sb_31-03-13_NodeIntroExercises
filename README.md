# sb_31-03-13_NodeIntroExercises -- Node Files

## Assignment Details
## Step 1: 
`step1.js` is a function that performs the `cat` function. `step1.js` takes a single argument, a file, and it writes the contents of the file to the console. Any errors encountered when accessing the file are written to the console and execution is halted.

## Step 2: 
`step2.js` builds on **Step 1** by adding in a `webCat` function. When a url is specified instead of a file, `webCat` goes to the url and prints a portion of the returned html to console.log. File functionality from **Step 1** still exists and either cat or webCat are called depending on the argument passed into `step2.js`.

## Step 3: 
`step3.js` builds on **Step 2** by adding an output file option, `--out output_file_name`, which when specified before the file/url to read, writes the output of the cat or webCat functions into file `output_file_name`. The console is used when the output file is not specified.


**Enhancements**

- For `step2.js`, only a portion of the returned html is written to the console. A message was also added to indicate the html may not be from the specified url but from an enhanced 404 error from a web provider.
- For `step3.js`:
  - Comments were added for cat and webCat function. 
  - Syntax help prints to console when `step3.js` is issued without any arguments. 
  - An error message was added when too few arguments were passed into `step3.js`. 
  - The `cat` and `webCat` function declarations were changed to include the addition of the output file passed in as a parameter. Instead of logging directly to the console, a function is called from within `cat` or `webCat` that writes either to the console when outfile is "" or it writes to the output file. Any errors are sent to the console.

