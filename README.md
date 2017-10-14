# Setup
```
cd /usr/local/lib
sudo curl -O http://www.antlr.org/download/antlr-4.7-complete.jar
export CLASSPATH=".:/usr/local/lib/antlr-4.7-complete.jar:$CLASSPATH"
alias antlr4='java -jar /usr/local/lib/antlr-4.7-complete.jar'
alias grun='java org.antlr.v4.gui.TestRig'
```
# Run
```
antlr4 Expr.g4
javac Expr*.java
grun Expr prog -gui inputs.txt
```
