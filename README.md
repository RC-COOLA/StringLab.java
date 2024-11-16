public class StringLab {
    public static void main(String[] args) {
String str = " Welcome to the Java String Lab! ";
        System.out.println("Length: " + str.length());

       
        System.out.println("Character at index 7: " + str.charAt(7));

       
        System.out.println("Substring 'Java': " + str.substring(18, 22));

       
        System.out.println("Uppercase: " + str.toUpperCase());
        System.out.println("Lowercase: " + str.toLowerCase());

    
        System.out.println("Index of 'Java': " + str.indexOf("Java"));

      
        System.out.println("Contains 'Lab': " + str.contains("Lab"));

     
        System.out.println("Replace 'Java' with 'Java Programming': " + str.replace("Java", "Java Programming"));

    
        String[] words = str.split(" ");
        System.out.println("Split words:");
        for (String word : words) {
            System.out.println(word);
        }

     
        System.out.println("Trimmed string: '" + str.trim() + "'");

    
        String compareStr = "java string lab!";
        System.out.println("Equals: " + str.equals(compareStr));
        System.out.println("EqualsIgnoreCase: " + str.equalsIgnoreCase(compareStr));

  

        StringBuilder sb = new StringBuilder("StringBuilder Lab");

 
        sb.append(" - Learning Java");
        System.out.println("After append: " + sb);


        sb.insert(sb.indexOf("Lab") + 3, " is fun");
        System.out.println("After insert: " + sb);

      
        int start = sb.indexOf("Learning");
        int end = start + "Learning".length();
        sb.delete(start, end);
        System.out.println("After delete: " + sb);

  
        sb.reverse();
        System.out.println("After reverse: " + sb);

        StringBuffer sbf = new StringBuffer("Multithreading Lab");

   
        sbf.append(" - Learning Java");
        System.out.println("After append: " + sbf);

   
        sbf.insert(sbf.indexOf("Lab") + 3, " is fun");
        System.out.println("After insert: " + sbf);

      
        start = sbf.indexOf("Learning");
        end = start + "Learning".length();
        sbf.delete(start, end);
        System.out.println("After delete: " + sbf);
        sbf.reverse();
        System.out.println("After reverse: " + sbf);
    }
}
