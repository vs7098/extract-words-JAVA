Java program to extract words from a given sentence

In this java program, we are going to learn how to extract words from a string? Here, we are reading a string (sentence) and extracting words from it.

Given a sentence (string) and we have to extract words from a string using java program.


/*Extract words from a string in java.*/
    
     class ExtractWordFromSentence
     {
	public static void main(String args[])
	{
		String str = "My Name Is Preeti Jain";
		String [] words = str.split(" ", 4);

		for (String word : words)
			System.out.println(word);
	}
     }
 
 ******* OUTPUT ****
     	
	$java ExtractWordFromSentence
	My
	Name
	Is
	Vinay
	Singh

