# 1214klim.c


## check.c 
我不確定是不是這樣寫，我手邊沒有可以用GCC編譯ㄉ東東
```c
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[]) {
  char *endptr = NULL;
  if(argc != 3){
      for (int i = 0; i < argc; ++i){
          printf("%s ",argv[i]);
      }
      printf("msg base\n");
      exit(1);
  }
  else{
    int val = strtol(argv[2], &endptr, 10);
        if(*endptr){
            for(int i = 0; i < 2; ++i){
                printf("%s ",argv[i]);
            }  
            printf("Bad base: %s\n", argv[2]);
            exit(1);
        }
        else{
            //checsum懶得寫，反正就是一個一個做，差低
        
        }
  }
  
  return 0;
}
```
--------------
## angle.c 
