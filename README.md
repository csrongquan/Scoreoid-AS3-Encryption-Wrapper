#Scoreoid-AS3-Encryption-Wrapper

A simple open source AS3 Scoreoid encryption wrapper done by Alex Bogartz from <a href="http://www.makaimedia.com/" title="Makai Media Inc" target="_blank">Makai Media Inc</a>.

##Usage
Big thanks to Alex Bogartz for releasing this example. Usage example also located at the class comments.

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

##Scoreoid
More info at - <a href="http://wiki.scoreoid.net/open-source-examples/scoreoid-as3-encryption-wrapper/" target="_blank">Scoreoid Wiki</a>
Scoreoid - <a href="http://www.scoreoid.net/" target="_blank">Scoreoid</a> 