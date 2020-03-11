title: Doing things in sequence

The SEQUENCE item has two important functions:

- It runs multiple other items one after another.
- It determines which items should, and which shouldn't, be run.

SEQUENCEs are run from top to bottom; that is, the item at the top is run first. The order of a SEQUENCE is always sequential.

## Run-if statements

You can use run-if statements to determine whether or not a particular item should be run. For example, if you want a display to be presented only if a participant has made an incorrect response, you can set the Run-if statement for that item to:

	[correct] = 0

If you leave the run-if statement empty or enter 'always', the item will always be run. Run-if statements use the same syntax as all OpenSesame conditional statements. For more information, see:

- %link:manual/variables%

Run-if statements only affect which items are run, not which items are prepared. Phrased differently, the Prepare phase of all items in a SEQUENCE is always executed, regardless of the run-if statement. See also:

- %link:prepare-run%
