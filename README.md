# python-program-to-find-the-most-frequent-words-from-a-file.

 41.CODING   
name = input('Enter file:')
handle =open(name,'r')
text = handle.read()
words = text.split()
counts = dict()
for word in words:
    counts[word] = counts.get(word,0) + 1
bigcount = None
bigword = None
for word,count in counts.items():
     if bigcount is None or count > bigcount:
         bigword = word
         bigcount = count
         print(bigword,bigcount)  


Output:
	
Enter file:24sbcs01


