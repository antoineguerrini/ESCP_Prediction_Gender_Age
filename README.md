NOTE TO PROFESSOR:

DUE TO COMPUTATIONAL POWER PROBLEMS, WE APPLY BOTH TRAIN AND TEST MODELING ON SEVERAL SUBSETS. IN FACT, PARTIONING WITH SEVERAL SAMPLE WAS EASIER TO ITERATE. PLEASE FIND IN THE FOLDER DATA THE DATASETS USED.

Demographic prediction


When a user visits (one of ) our websites, we collect information about keywords extracted from
the website's url. For each user, the frequency of visits per keyword per day is also stored. For
example, suppose that a given user has visited the two following sites recently:
html://mypage/abc-news/aaa-bbb.html
html://mypage/news/aaa.html
The keywords (that have been) “seen” by the user will be then stored as follows (semicolon is
used to separate words):
abc:1;news:2;aaa:2;bbb:1;mypage:2
Thanks to external data (or some sources of data bought by our marketing department), we have
demographic information (like age, sex, race, ...) on about 5% of our visitors. The Head of
Product wanted to predict demographics (age, sex) for the rest of our visitors from the keywords
collected. He then spoke to Mr. Google, who advised him to hire a talented Master student from
ESCP Europe, in order to transform his idea into reality. And now, you understand why we are
contacting you ...
The Head of Product's asked you to build a machine learning model to predict age and sex for
each line in our dataset, which was partially extracted from one month's data (the portion of each
day's data was concatenated). The dataset contains two files named train.csv (to help you train
your model) and test.csv. Its format looks like: userID, keywords, age, sex (comma is used as a
delimiter). Note that there are some missing data in our dataset, and we removed all the “labels”
(age, sex) from the test file.
Once your model is built, you have to use the test.csv file to test your model, and send us the
results as a csv file containing only three columns: ID, age_pred, sex_pred. For example, your
submission file should look like:
ID,age_pred,sex_pred
1,35,F
2,45,M
...
You must also send us your solution/code via github.

