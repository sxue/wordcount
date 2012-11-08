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
//using System;
 public class WordCountEntry
{
static public void Main()
{
Console.WriteLine( "Beginning WordCount program ... " );
WordCount theObj = new WordCount();
theObj.processFile();
Console.WriteLine( "Ending WordCount program ... " );
}
}