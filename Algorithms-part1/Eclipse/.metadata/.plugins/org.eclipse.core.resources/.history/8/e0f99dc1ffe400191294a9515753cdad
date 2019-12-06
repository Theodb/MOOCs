package fr.theodb.interviewquestionweek1;

//Quick Union with path compression

public class SocialNetwork{
    public void main(String[] args){
 
    }
 
    public class QuickUnionUF
    {
        private int[] id;
        private int nCount;
        private boolean connected;
 
        public QuickUnionUF(int n)
        {
            nCount = n;
            connected = false;
            id = new int[n];
            for(int i = 0; i < n; i++){
                id[i] = i;
            }
        }
        
        private int root(int i){
            while(i != id[i]){
               id[i] = id[id[i]]; //Path compression
               i = id[i];
            }
            return i;
        }
        
        public boolean connected(int p, int q){
            return root(p) == root(q);
        }
 
        public boolean friendconnection(int p, int q){
            int i = root(p);
            int j = root(q);
            id[i] = j;
            return connected;
        }
    }
}