All Old Practiced cpommands

awk command : It is used to pick or list columns from output   

$NF means last Column ;  NR means no of rows  ; NF no of Columns or fields ; $o is used to print row

Examples : 
1. awk '{print $1 }' <File> -> for printing 1st comlun
2. awk '{print $NF}' <file> -> to print last Column of a table
3. awk '{print NR ":" $4 }' -> to print no of rows with semicolon and the column
4. ll | awk '{ if($2>"2"){$2="0"} print $O}' : here were listing and changing the cloumn second value using awk
5. awk '/SearchString/{print $o }' : for find a string and printing the line for matched rows

cut command :- It is used to words of output 

1. echo "hello-Elephant" | cut -c2    : will return the 2nd alphabet of the word
   output : e
2. echo "hello-Elephant" | cut -c2-4  : will output the range of the given word
   output : ell
3. echo "hello-Elephant" | cut -c2,4  : will output the specified words
   output : el
4. cut -d -f --output-delimeter="%"

