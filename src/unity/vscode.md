# VSCode

We use [VSCode](https://code.visualstudio.com/) as our primary code editor for unity.
- Be sure to install the C# for Visual Studio Code(omnisharp) from the VSCode extensions tab.
- Be sure to have our omnisharp C# code styling file:
```bash
cd ~
mkdir .omnisharp # Don't forget the dot in .omnisharp
touch .omnisharp/omnisharp.json
```
And copy this code to it:
```
{
  "FormattingOptions": {
    "NewLinesForBracesInTypes": false,
    "NewLinesForBracesInMethods": false,
    "NewLinesForBracesInProperties": false,
    "NewLinesForBracesInAccessors": false,
    "NewLinesForBracesInAnonymousMethods": false,
    "NewLinesForBracesInControlBlocks": false,
    "NewLinesForBracesInAnonymousTypes": false,
    "NewLinesForBracesInObjectCollectionArrayInitializers": false,
    "NewLinesForBracesInLambdaExpressionBody": false,
    "NewLineForElse": false,
    "NewLineForCatch": false,
    "NewLineForFinally": false,
    "NewLineForMembersInObjectInit": false,
    "NewLineForMembersInAnonymousTypes": false,
    "NewLineForClausesInQuery": false,
    "UseTabs": false,
    "TabSize": 2,
    "IndentationSize": 2
  }
}
```
