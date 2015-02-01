

int read(char *buf, int n){
  int res=0;
  char[5] localBuf;
  do{
    int k = read4(localBuf);
    if(res+k<n){
      res+=k;
      strncpy(buf, localBuf, k); 
    } else {
      strncpy(buf, localBuf, n-res);
      return n;
    }
    if(k<4) break;
  }while(true);
  return res;
}
