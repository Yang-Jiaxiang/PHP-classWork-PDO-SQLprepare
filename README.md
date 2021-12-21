# PHP-classWork-PDO-SQLprepare

$link = new PDO('mysql:host='.$hostname.';dbname='.$database.';charset=utf8', $username, $password);

		// 用SQL語法呼叫mysql_query()
		$query ="select * from `person` where `user`=? and `pwd`=?";
		$result = $link->prepare($query);
		$exeres = $result->execute(array($user, $pwd));
		if ($exeres){
    
    }
