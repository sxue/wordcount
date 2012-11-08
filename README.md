wordcount
=========
using System;
public class WordCount
{
public void processFile()
{
openFiles();
readFile();
countWords();
writeWords();
}
private void countWords()
{
Console.WriteLine( "!!! WordCount.countWords()" );
}
private void readFile()
{
Console.WriteLine( "!!! WordCount.readFile()" );
}
private void openFiles()
{
Console.WriteLine( "!!! WordCount.openFiles()" );
}
private void writeWords()
{
Console.WriteLine( "!!! WordCount.writeWords()" );
}
}
 public class WordCountEntry
{
   static void Main(string[] args)
  { 
    if (args.Length==0)
   {
    display_usage();
    return ; 
    }
bool traceOn=false;
bool spYOn=false;
foreach ( string option in args )
{
  if (option.Equals("-t"))
      traceOn=true;
else
if(option.Equals("-s"))
spyOn=true;
else
if(option.Equals("-h"))
{display_usage();
 return;
}
else
check_valid_file_type(option);
}
Console.WriteLine( "Beginning WordCount program ... " );
WordCount theObj = new WordCount();
theObj.processFile();
Console.WriteLine( "Ending WordCount program ... " );
}
}
