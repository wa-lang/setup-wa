# Setup Wa Language

```yaml
name: Test
on: push
jobs:
  build:
    name: Run Wa App
    runs-on: ubuntu-latest
    steps:
      - name: Git checkout
        uses: actions/checkout@v2

      - name: Set up Wa(凹语言)
        uses: wa-lang/setup-wa

      - run: wa -v
      - run: wa run heart.wa
```

Output:

```text
$ wa run heart.wa
                                           
                                           
            @@@@@@        @@@@@@           
        @@@@@@@@@@@@@ @@@@@@@@@@@@@@       
       @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@      
      @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@     
      @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@     
      @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@     
      @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@     
       @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@      
        @@@@@@@@@@@@@@@@@@@@@@@@@@@@       
         @@@@@@@@@@@@@@@@@@@@@@@@@@        
          @@@@@@@@@@@@@@@@@@@@@@@          
            @@@@@@@@@@@@@@@@@@@@           
               @@@@@@@@@@@@@@              
                  @@@@@@@@                 
                     @@                    
```
