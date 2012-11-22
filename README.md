wordcount
=========
using System;
using System.IO;
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
/*  string text_line;
	while ((text_line=freader.ReadLine() )!=null)
	{
		//write to output file
		fwriter.WriteLine(text_line );
	}
	//must explicitly close the readers
	freader.Close();
	fwrriter.Close();*/
Console.WriteLine( "!!! WordCount.readFile()" );
}
private void openFiles()
{
  string file_name=@"a.txt";
 StreamReader freader=File.OpenText(file_name);
 StreamWriter fwriter=File.CreateText(@"a.diag");
/* {
	 public static void display_usage()
	{
	string usage=

		@"usage:WordCount[-s] [-t] [-h] textfile.txt
		where[] indicates an optional argument
		-s prints a series of performance measurements
		-t prints a trace of the program
		-h prints this message";
	Console.WriteLine(usage);
}
//CoConsole.WriteLine( "!!! WordCount.openFiles()" );
}*/
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
    else

bool traceOn=false;嵌入的语句不能是声明或标记语句
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