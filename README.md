# ThreadExtractor
The thread extractor is used to extract all threads from email.
Please refer to email-thread-extractor.pdf for detailed implementation.
You can use this extractor by:

from extractor import Extractor
result = Extractor.extract(text)

The text is the email string you want to extract threads from, the result is the extraction output.

result[0] contains all the thread body in chronological order.

result[1] contains all the thread head in chronological order.

Both thread body and head are stored as a tuple [char position of start index,text]
