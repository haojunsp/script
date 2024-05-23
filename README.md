Read me:

The steps for using the script in conjunction with the Silva database are as follows:

Step 1: Prepare the SSU rRNA gene. Evaluate the universal primers in the Silva database, and then download a SSU rRNA gene sequence from the target microorganism that is not covered by the universal primers and place it in the “gene” folder. Specifically: (1) Log in to the website https://www.arb-silva.de/search/testprime. (2) Enter the primer sequence, then click “Run TestPrime”, followed by “Inspect Results in Taxonomy Browser”. (3) Click on the species that are not covered, which marked in black. (4) Click “Fasta” to download the sequences.

Step 2: Prepare the primers. Place the forward primer (F primer) and reverse primer (R primer) of the universal primers to be improved into the “old F” and “old R” folders, respectively.

Step 3: Run the commands. Execute the “script F” or “script R” command in the macOS terminal or Linux shell.

Step 4: Collect the new primers. The new primers will be displayed in the running interface and in the "new F/R" folder. Replace the old primers with the new ones and repeat steps 1-4 for iterative improvement until Silva indicates that the new primers are invalid due to containing multiple degenerate bases, resulting in more than 60 primer sequences. The last round of effective primers is considered the final improved primers.


Note:
1. In the initial state, gene and primer data for demonstration have already been placed in the folder, which can be used to test whether the script is functioning properly. Each time researchers use the script, they need to remove old files from "gene", "old_F", and "old_R", and replace them with new files.

2. Considering the impact of gene length on processing speed, the SSU rRNA gene should be extracted from the genomic sequence when dealing with genomic data.

3. File names should not contain special characters such as "<", ">", "?", "*", "/", etc. Avoid using "." as the first character of the file name.

4. The reference for this script is "Developing the script 'Degenerate primer 111' to enhance the coverage of universal primers for the small subunit rRNA gene on target microorganisms".

5. If there are any questions during the use, please feel free to contact the author via email at 11807011@zju.edu.cn.
