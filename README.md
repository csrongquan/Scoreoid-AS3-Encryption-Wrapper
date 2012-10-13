#Scoreoid AS3 Encryption Wrapper

A simple open source AS3 Scoreoid encryption wrapper done by Alex Bogartz from <a href="http://www.makaimedia.com/" title="Makai Media Inc" target="_blank">Makai Media Inc</a>.

##Usage
Big thanks to Alex Bogartz for releasing this example. Usage example also located at the class comments.

```actionscript
public function getGame():void
{
    var scoreoidEnc:ScoreoidEncryption=new ScoreoidEncryption(apikey,gameID,key)
    var params={limit:3, order_by:"score",order:"desc"}
    scoreoidEnc.sendData("https://www.scoreoid.com/api/getScores",params)
}

public function submitScore(score:Number):void
{
   var scoreoidEnc:ScoreoidEncryption=new ScoreoidEncryption(apikey,gameID,key); 
   var params={username:user.name, score:score}
   scoreoidEnc.sendData("https://www.scoreoid.com/api/createScore",params)
}
```
##Scoreoid Links
<a href="http://wiki.scoreoid.net/" target="_blank">Scoreoid Wiki</a>.  
<a href="http://wiki.scoreoid.net/category/user-guide/" target="_blank">User Guide</a>.  
<a href="http://wiki.scoreoid.net/category/api/" target="_blank">Scoreoid API</a>.  
<a href="http://wiki.scoreoid.net/category/open-source-examples/" target="_blank">Open Source Examples</a>.  
<a href="http://wiki.scoreoid.net/category/3rd-party-tutorials/" target="_blank">Tutorials</a>.    
<a href="http://www.scoreoid.net/" target="_blank">Scoreoid  Website</a>.  
<a href="http://www.scoreoid.net/support/" target="_blank">Scoreoid  Support</a>.  
<a href="https://trello.com/board/scoreoid-public-development-roadmap/4f97c80855ed960f672d7f88" target="_blank">Public Roadmap on Trello</a>.  
<a href="http://www.scoreoid.net/category/featured-developers/" target="_blank">Developer Interviews</a>.