# Writing evaluation data science project

The dataset contains argumentative essays written by U.S students in grades 6-12. The essays were annotated by expert raters for elements commonly found in argumentative writing.

Note that this is a code competition, in which you will submit code that will be run against an unseen test set. The unseen test set is approximately 10k documents. A small public test sample has been provided for testing your notebooks.

Your task is to predict the human annotations. You will first need to segment each essay into discrete rhetorical and argumentative elements (i.e., discourse elements) and then classify each element as one of the following:

* **Lead** - an introduction that begins with a statistic, a quotation, a description, or some other device to grab the reader’s attention and point toward the thesis
* **Position** - an opinion or conclusion on the main question
* **Claim** - a claim that supports the position
* **Counterclaim** - a claim that refutes another claim or gives an opposing reason to the position
* **Rebuttal** - a claim that refutes a counterclaim
* **Evidence** - ideas or examples that support claims, counterclaims, or rebuttals.
* **Concluding Statement** - a concluding statement that restates the claims
The training set will consist of individual essays in a folder of .txt files, as well as a .csv file containing the annotated version of these essays. It is important to note that some parts of the essays will be unannotated (i.e., they do not fit into one of the classifications above).

Files

* train.zip - folder of individual .txt files, with each file containing the full text of an essay response in the training set
* train.csv - a .csv file containing the annotated version of all essays in the training set
* id - ID code for essay response
* discourse_id - ID code for discourse element
* discourse_start - character position where discourse element begins in the essay response
* discourse_end - character position where discourse element ends in the essay response
* discourse_text - text of discourse element
* discourse_type - classification of discourse element
* discourse_type_num - enumerated class label of discourse element
* predictionstring - the word indices of the training sample, as required for predictions
* test.zip - folder of individual .txt files, with each file containing the full text of an essay response in the test set
* sample_submission.csv - file in the required format for making predictions - note that if you are making multiple predictions for a document, submit multiple rows

