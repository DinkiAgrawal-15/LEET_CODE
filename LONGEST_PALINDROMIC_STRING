public class Solution {
    public String longestPalindrome(String s) {
        String longest = "";
        for (int i = 0; i < s.length(); i ++){
            String tmp = "";
            tmp = paCenterBy(s, i, i);
            if (tmp.length() > longest.length()){
                longest = tmp;
            }
            tmp = paCenterBy(s, i, i + 1);
            if (tmp.length() > longest.length()){
                longest = tmp;
            }
        }  
        return longest;
    }
    private String paCenterBy(String s, int cleft, int cright){
        String result = "";
        while (cleft >=0 && cright < s.length() && s.charAt(cleft) == s.charAt(cright)){
            cleft --;
            cright ++;
        }
        return s.substring(cleft + 1, cright);
    }
}
