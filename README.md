# timebank_dense_with_word_embeddings
Dataset of word embeddings for the events in TimeBank 1.2

To use word embeddings for temporal classification, you would need access to TimeBank 1.2, TimeBank-Dense and Word2Vec pretrained vectors. 

TimeBank 1.2
http://www.timeml.org/timebank/documentation-1.2.html

TimeBank-Dense
https://www.usna.edu/Users/cs/nchamber/caevo/#corpus

Word2Vec Model
https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/

This dataset will greatly reduce effort as it combines the information from these three.

TimeBank 1.2 contains:
Total EVENT tags 7935
Unique EVENT tags 764
Out of these 764 unique tags , 117 tags are not found in Word2Vec pre-trained vectors (most of them are numbers or words joined by '-' e.g. 'high-flying')
Hence the dataset contains word embeddings for 764-117 = 647 EVENTs

Structure:
dataset contains 647 rows. Each row has 303 columns.
1st col: timebank-filename
2nd col: event-id
3rd col: event-word
4-303 col: event-word-vector (dimension 300)


