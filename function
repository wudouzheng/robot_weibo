function post_tweet($cookies_global,$text_data_post,$pic_id_data_post,$user_data_array_global)
{
	//函数功能：发布微博内容
	//输入参数1：cookies
	//输入参数2:发布的内容
	//输入参数3:图片的编号
	//输入参数4:用户数据数组
	//输出参数：状态吗
	
	
	//variable of public 
	$url_post; 
	$curl; 
	$result; 
	$user_data_array_global; 
	
	
	//variable of header in post.
	$headers_post;
	$referer_headers_post;
	$userAgent_headers_post;
	$cookies_headers_post;
	$origin_headers_post;
	$acceptEncoding_headers_post;
	$acceptLanguage_headers_post;
	$contentType_headers_post;
	$accept_headers_post;
	$xRequestedWith_headers_post;
	$connection_headers_post;
	
	//variable of data in post.
	$data_post;
	$text_data_post;
	$location_data_post;
	$text_data_post;
	$appkey_data_post;
	$style_type_data_post;
	$pic_id_data_post;
	$tid_data_post;
	$pdetail_data_post;
	$mid_data_post;
	$isReEdit_data_post;
	$rank_data_post;
	$rankid_data_post;
	$module_data_post;
	$pub_source_data_post;
	$pub_type_data_post;
	$isPri_data_post;
	$_t_data_post;
	

	
	
	//header的值
	$url_post = 'https://weibo.com/aj/mblog/add?ajwvr=6&__rnd='.$user_data_array_global[15];
	$referer_headers_post = 'Referer: https://weibo.com/'.$user_data_array_global[10].'/home?topnav=1&wvr=6&mod=logo';
	$userAgent_headers_post = 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/66.0.3359.170 Safari/537.36';
	$cookies_headers_post = $cookies_global;
	$origin_headers_post = 'Origin: https://weibo.com';
	$acceptEncoding_headers_post = 'Accept-Encoding: gzip, deflate, br';
	$acceptLanguage_headers_post = 'Accept-Language: zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7';
	$contentType_headers_post = 'Content-Type: application/x-www-form-urlencoded';
	$accept_headers_post = 'Accept: */*';
	$xRequestedWith_headers_post = 'X-Requested-With: XMLHttpRequest';
	$connection_headers_post = 'Connection: keep-alive';
	
	//含有header值的数组
	$headers_post = array($cookies_headers_post,$origin_headers_post,$acceptEncoding_headers_post,$acceptLanguage_headers_post,$userAgent_headers_post,$contentType_headers_post,$accept_headers_post,$referer_headers_post,$xRequestedWith_headers_post,$connection_headers_post);
	
	
	
	//data的值
	$location_data_post = 'location=v6_content_home';
	$text_data_post = $text_data_post;
	$appkey_data_post = '&appkey=';
	$style_type_data_post = '&style_type=1';
	$pic_id_data_post = $pic_id_data_post;
	$tid_data_post = '&tid=';
	$pdetail_data_post = '&pdetail=';
	$mid_data_post = '&mid=';
	$isReEdit_data_post = '&isReEdit=false';
	$rank_data_post = '&rank=0';
	$rankid_data_post = '&rankid=';
	$module_data_post = '&module=stissue';
	$pub_source_data_post = '&pub_source=main_';
	$pub_type_data_post = '&pub_type=dialog';
	$isPri_data_post = '&isPri=0';
	$_t_data_post = '&_t=0';
	
	//含有data值的串联变量.
	$data_post = $location_data_post.$text_data_post.$appkey_data_post.$style_type_data_post.$pic_id_data_post.$tid_data_post.$pdetail_data_post.$mid_data_post.$isReEdit_data_post.$rank_data_post.$rankid_data_post.$module_data_post.$pub_source_data_post.$pub_type_data_post.$isPri_data_post.$_t_data_post;
	







	
	
	
	$curl = curl_init();
	curl_setopt($curl, CURLOPT_URL, $url_post);
	curl_setopt($curl, CURLOPT_ENCODING, ""); //禁止curl数据压缩。
	curl_setopt($curl, CURLOPT_POST, 1);
	curl_setopt($curl, CURLOPT_HEADER, true);
	curl_setopt ($curl, CURLOPT_HTTPHEADER , $headers_post);
	curl_setopt($curl, CURLOPT_POSTFIELDS, $data_post);
	curl_setopt ($curl, CURLOPT_RETURNTRANSFER, 1);//结果不直接输出到浏览器

	$result = curl_exec($curl);
	
	curl_close($curl);
	
return $result;
}

function post_upload_tweet($cookies_global,$jpeg_data_post,$user_data_array_global)
{
		//函数功能：上传图片到微博tweet
	//输入参数1:cookies
	//输入参数2:图片数据
	//输入参数3:用户数据
	
	//输出参数：上传图片后的html数据
	
		
	$url_post;//Var url of post.
	$curl;//var curl.
	$user_data_array_global;
	$result;//var out.
	
	
	
	//Var header of post.
	$headers_post;
	$referer_headers_post;
	$userAgent_headers_post;
	$cookies_headers_post;
	$origin_headers_post;
	$acceptEncoding_headers_post;
	$acceptLanguage_headers_post;
	$contentType_headers_post;
	$accept_headers_post;
	$xRequestedWith_headers_post;
	$connection_headers_post;
	
	$cacheControl_headers_post;
	$host_headers_post;
	$upgradeInsecureRequests_headers_post;

 
//Content-Length: 283883

 
	$url_post = 'https://picupload.weibo.com/interface/pic_upload.php?cb=https%3A%2F%2Fweibo.com%2Faj%2Fstatic%2Fupimgback.html%3F_wv%3D5%26callback%3DSTK_ijax_'.$user_data_array_global[15].'&mime=image%2Fjpeg&data=base64&url=0&markpos=1&logo=&nick=0&marks=0&app=miniblog&s=rdxt&pri=null&file_source=1';
	$referer_headers_post = 'Referer: https://weibo.com/'.$user_data_array_global[10].'/home?wvr=5';
	$userAgent_headers_post = 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/66.0.3359.170 Safari/537.36';
	$cookies_headers_post = $cookies_global;
	$origin_headers_post = 'Origin: https://card.weibo.com';
	$acceptEncoding_headers_post = 'Accept-Encoding: gzip, deflate, br';
	$acceptLanguage_headers_post = 'Accept-Language: zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7';
	$contentType_headers_post = 'Content-Type: application/x-www-form-urlencoded';
	$accept_headers_post = 'Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8';
	$xRequestedWith_headers_post = 'X-Requested-With: XMLHttpRequest';
	$connection_headers_post = 'Connection: keep-alive';

	$cacheControl_headers_post = 'Cache-Control: max-age=0';
	$host_headers_post = 'Host: picupload.weibo.com';
	$upgradeInsecureRequests_headers_post = 'Upgrade-Insecure-Requests: 1';
	
	//含有header值的数组
	$headers_post = array($cookies_headers_post,$origin_headers_post,$acceptEncoding_headers_post,$acceptLanguage_headers_post,$userAgent_headers_post,$contentType_headers_post,$accept_headers_post,$referer_headers_post,$xRequestedWith_headers_post,$connection_headers_post,$cacheControl_headers_post,$host_headers_post,$upgradeInsecureRequests_headers_post);
	
	
		//var data of post.
	$data_post;
	$jpeg_data_post;
	$base64_jpeg_data_post;
	$urlencode_base64_jpeg_data_post;

	$jpeg_data_post = file_get_contents($jpeg_data_post);// picture include
	$base64_jpeg_data_post = base64_encode($jpeg_data_post);//base64 encode of picture
	$urlencode_base64_jpeg_data_post = urlencode($base64_jpeg_data_post);//url encode of base64 of picture
	$data_post = 'b64_data='.$urlencode_base64_jpeg_data_post;
	
	
	

	
	
	$url_post = 'https://picupload.weibo.com/interface/pic_upload.php?cb=https%3A%2F%2Fweibo.com%2Faj%2Fstatic%2Fupimgback.html%3F_wv%3D5%26callback%3DSTK_ijax_'.$user_data_array_global[15].'&mime=image%2Fjpeg&data=base64&url=0&markpos=1&logo=&nick=0&marks=0&app=miniblog&s=rdxt&pri=null&file_source=1';
	$curl = curl_init();
	curl_setopt($curl, CURLOPT_ENCODING, ""); //禁止curl数据压缩。
	curl_setopt($curl, CURLOPT_URL, $url_post);
	curl_setopt($curl, CURLOPT_POST, 1);
	curl_setopt($curl, CURLOPT_HEADER, true);//输出响应头
	curl_setopt ($curl, CURLOPT_HTTPHEADER , $headers_post);
	curl_setopt($curl, CURLOPT_RETURNTRANSFER, TRUE);
	curl_setopt($curl, CURLOPT_POSTFIELDS, $data_post);
	curl_setopt ($curl, CURLOPT_RETURNTRANSFER, 1);//结果不直接输出到浏览器
	//curl_setopt($curl, CURLOPT_FOLLOWLOCATION, 1);
	

	$result = curl_exec($curl);
	//$result = curl_getinfo($curl,CURLINFO_CONTENT_TYPE); 
	curl_close($curl);
	
	
	return $result;
	
	
	
	
	
	
}




function post_comment($cookies_global,$mid_data_post,$content_data_post,$user_data_array_global)
{
	//函数功能：评论微博帖子
	//输入参数1:cookies
	//输入参数2:目标帖子id
	//输入参数3:评论内容
	//输入参数4:用户数据
	
	//输出参数：状态码
	
	$url_post;//Var url of post.
	$curl;//var curl.
	$result;//var out.
	$user_data_array_global;
	
	
	//Var header of post.
	$headers_post;
	$referer_headers_post;
	$userAgent_headers_post;
	$cookies_headers_post;
	$origin_headers_post;
	$acceptEncoding_headers_post;
	$acceptLanguage_headers_post;
	$contentType_headers_post;
	$accept_headers_post;
	$xRequestedWith_headers_post;
	$connection_headers_post;
	$contentLength_headers_post;
	
	//var data of post.
	$data_post;
	$text_data_post;
	$location_data_post;
	$text_data_post;
	$appkey_data_post;
	$style_type_data_post;
	$pic_id_data_post;
	$tid_data_post;
	$pdetail_data_post;
	$mid_data_post;
	$isReEdit_data_post;
	$rank_data_post;
	$rankid_data_post;
	$module_data_post;
	$pub_source_data_post;
	$pub_type_data_post;
	$isPri_data_post;
	$_t_data_post;
	


	
	//header的值
	$url_post = 'https://weibo.com/aj/v6/comment/add?ajwvr=6&__rnd='.$user_data_array_global[15];
	$referer_headers_post = 'Referer: https://weibo.com/'.$user_data_array_global[10].'/profile?rightmod=1&wvr=6&mod=personnumber&is_all=1';//不同的账号需要不同的来源
	$userAgent_headers_post = 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/66.0.3359.170 Safari/537.36';
	$cookies_headers_post = $cookies_global;
	$origin_headers_post = 'Origin: https://weibo.com';
	$acceptEncoding_headers_post = 'Accept-Encoding: gzip, deflate, br';
	$acceptLanguage_headers_post = 'Accept-Language: zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7';
	$contentType_headers_post = 'Content-Type: application/x-www-form-urlencoded';
	$accept_headers_post = 'Accept: */*';
	$xRequestedWith_headers_post = 'X-Requested-With: XMLHttpRequest';
	$connection_headers_post = 'Connection: keep-alive';
	//$contentLength_headers_post='Content-Length: 375';//计算发布的post数字
	
	//含有header值的数组
	$headers_post = array($cookies_headers_post,$origin_headers_post,$acceptEncoding_headers_post,$acceptLanguage_headers_post,$userAgent_headers_post,$contentType_headers_post,$accept_headers_post,$referer_headers_post,$xRequestedWith_headers_post,$connection_headers_post);
	
	
	
	//data的值
	$act_data_post = 'act=post';
	$mid_data_post = $mid_data_post;//目标帖子id
	$uid_data_post = '&uid='.$user_data_array_global[6];//本账号id
	$forward_type_data_post = '&forward=0';
	$isroot_id_data_post = '&isroot=0';
	$content_data_post = $content_data_post;//内容
	$location_data_post = '&location=page_100505_home';//不同的账号有不同的location
	$module_data_post = '&module=scommlist';
	$group_source_data_post = '&group_source=';
	$pdetail_data_post = '&pdetail=1005053571522617';//不同的页面会有页面id
	$_t_data_post = '&_t=0';
	
	
	//含有data值的串联变量.
	$data_post = $act_data_post.$mid_data_post.$uid_data_post.$forward_type_data_post.$isroot_id_data_post.$content_data_post.$location_data_post.$module_data_post.$group_source_data_post.$pdetail_data_post.$_t_data_post;
	


	
	
	
	$curl = curl_init();
	curl_setopt($curl, CURLOPT_URL, $url_post);
	curl_setopt($curl, CURLOPT_ENCODING, ""); //禁止curl数据压缩。
	curl_setopt($curl, CURLOPT_POST, 1);
	curl_setopt($curl, CURLOPT_HEADER, true);
	curl_setopt ($curl, CURLOPT_HTTPHEADER , $headers_post);
	curl_setopt($curl, CURLOPT_POSTFIELDS, $data_post);
	curl_setopt ($curl, CURLOPT_RETURNTRANSFER, 1);//结果不直接输出到浏览器

	$result = curl_exec($curl);
	
	curl_close($curl);
	
return $result;
	
	
}

function post_save_headarticle($cookies_global,$id_data_post,$title_data_post,$summary_data_post,$content_data_post,$cover_data_post,$user_data_array_global)
{
	//函数功能：保存微博头条文章
	//输入参数1：cookies
	//输入参数2:帖子id
	//输入参数3:标题
	//输入参数4：导语
	//输入参数5：内容
	//输入参数6：封面
	//输入参数7:用户数据
	
	//输出参数：状态码
	/*
	 * 
	 * id=42962&title=大标题&updated=2018-05-17 16:44:33&subtitle=&type=&free_content=&content=<p>内容</p>&cover=https://wx2.sinaimg.cn/large/d4e11c39gy1fn73818jrxj20xc0f5jyt.jpg&summary=导语&writer=&extra={}&is_word=0
	 * 
	 * 
	 * 
	 * 
	 * 
	 * */
	
	$url_post;//Var url of post.
	$curl;//var curl.
	$result;//var out.
	$user_data_array_global;
	
	
	//Var header of post.
	$headers_post;
	$referer_headers_post;
	$userAgent_headers_post;
	$cookies_headers_post;
	$origin_headers_post;
	$acceptEncoding_headers_post;
	$acceptLanguage_headers_post;
	$contentType_headers_post;
	$accept_headers_post;
	$xRequestedWith_headers_post;
	$connection_headers_post;
	
	

	
	$url_post = 'https://card.weibo.com/article/v3/aj/editor/draft/save';
	$referer_headers_post = 'Referer: https://card.weibo.com/article/v3/editor';
	$userAgent_headers_post = 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/66.0.3359.170 Safari/537.36';
	$cookies_headers_post = $cookies_global;
	$origin_headers_post = 'Origin: https://card.weibo.com';
	$acceptEncoding_headers_post = 'Accept-Encoding: gzip, deflate, br';
	$acceptLanguage_headers_post = 'Accept-Language: zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7';
	$contentType_headers_post = 'Content-Type: application/x-www-form-urlencoded';
	$accept_headers_post = 'Accept: application/json, text/plain, */*';
	$xRequestedWith_headers_post = 'X-Requested-With: XMLHttpRequest';
	$connection_headers_post = 'Connection: keep-alive';
	
	
	//含有header值的数组
	$headers_post = array($cookies_headers_post,$origin_headers_post,$acceptEncoding_headers_post,$acceptLanguage_headers_post,$userAgent_headers_post,$contentType_headers_post,$accept_headers_post,$referer_headers_post,$xRequestedWith_headers_post,$connection_headers_post);
	
	
	
	
	//var data of post.
	$data_post;
	$id_data_post;
	$title_data_post;
	$update_data_postd;
	$subtitle_data_post;
	$type_data_post;
	$free_content_data_post;
	$content_data_post;
	$summary_data_post;
	$cover_data_post;
	$writer_data_post;
	$is_word_data_post;
	
	
	
	$id_data_post = $id_data_post;
	$title_data_post = $title_data_post;
	$update_data_postd = '&updated='.date('Y-m-d').'%2016%3A44%3A33';//中间插入动态时间函数
	$subtitle_data_post = '&subtitle=';
	$type_data_post = '&type=';
	$free_content_data_post = '&free_content=';
	$content_data_post = $content_data_post;
	$cover_data_post = $cover_data_post;
	$summary_data_post = $summary_data_post;
	$writer_data_post = '&writer=';
	$extra = '&extra=%7B%7D';
	$is_word_data_post = '&is_word=0';
	$data_post = $id_data_post.$title_data_post.$update_data_postd.$subtitle_data_post.$type_data_post.$free_content_data_post.$content_data_post.$cover_data_post.$summary_data_post.$writer_data_post.$extra.$is_word_data_post;
	//含有data值的串联变量.
	
		/*
	 * 
	 * id=42962&title=%E5%A4%A7%E6%A0%87%E9%A2%98&updated=2018-05-17%2016%3A44%3A33&subtitle=&type=&free_content=&content=%3Cp%3E%E5%86%85%E5%AE%B9%3C%2Fp%3E&cover=https%3A%2F%2Fwx2.sinaimg.cn%2Flarge%2Fd4e11c39gy1fn73818jrxj20xc0f5jyt.jpg&summary=%E5%AF%BC%E8%AF%AD&writer=&extra=%7B%7D&is_word=0
	 */
	
	
	
	
	
	
	

	
	
	$url_post = 'https://card.weibo.com/article/v3/aj/editor/draft/save';
	$curl = curl_init();
	curl_setopt($curl, CURLOPT_ENCODING, ""); //禁止curl数据压缩。
	curl_setopt($curl, CURLOPT_URL, $url_post);
	curl_setopt($curl, CURLOPT_POST, 1);
	//curl_setopt($curl, CURLOPT_HEADER, true);//禁止输出响应头
	curl_setopt ($curl, CURLOPT_HTTPHEADER , $headers_post);
	curl_setopt($curl, CURLOPT_POSTFIELDS, $data_post);
	curl_setopt ($curl, CURLOPT_RETURNTRANSFER, 1);//结果不直接输出到浏览器

	$result = curl_exec($curl);
	
	curl_close($curl);
	
	
	return $result;
	
	
}

function post_publish_headarticle($cookies_global,$id_data_post,$text_data_post,$user_data_array_global)
{
	//函数功能：发布微博头条文章
	//输入参数1：cookies
	//输入参数2:帖子id
	//输入参数3:内容
	//输入参数4:用户数据

	
	//输出参数：状态码
	/*
	 * 
	 * id=42962&title=大标题&updated=2018-05-17 16:44:33&subtitle=&type=&free_content=&content=<p>内容</p>&cover=https://wx2.sinaimg.cn/large/d4e11c39gy1fn73818jrxj20xc0f5jyt.jpg&summary=导语&writer=&extra={}&is_word=0
	 * 
	 * 
	 * 
	 * 
	 * 
	 * */
	
	$url_post;//Var url of post.
	$curl;//var curl.
	$result;//var out.
	$user_data_array_global;
	
	
	//Var header of post.
	$headers_post;
	$referer_headers_post;
	$userAgent_headers_post;
	$cookies_headers_post;
	$origin_headers_post;
	$acceptEncoding_headers_post;
	$acceptLanguage_headers_post;
	$contentType_headers_post;
	$accept_headers_post;
	$xRequestedWith_headers_post;
	$connection_headers_post;
	
	

	
	$url_post = 'https://card.weibo.com/article/v3/aj/editor/draft/publish';
	$referer_headers_post = 'Referer: https://card.weibo.com/article/v3/editor';
	$userAgent_headers_post = 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/66.0.3359.170 Safari/537.36';
	$cookies_headers_post = $cookies_global;
	$origin_headers_post = 'Origin: https://card.weibo.com';
	$acceptEncoding_headers_post = 'Accept-Encoding: gzip, deflate, br';
	$acceptLanguage_headers_post = 'Accept-Language: zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7';
	$contentType_headers_post = 'Content-Type: application/x-www-form-urlencoded';
	$accept_headers_post = 'Accept: application/json, text/plain, */*';
	$xRequestedWith_headers_post = 'X-Requested-With: XMLHttpRequest';
	$connection_headers_post = 'Connection: keep-alive';
	
	
	//含有header值的数组
	$headers_post = array($cookies_headers_post,$origin_headers_post,$acceptEncoding_headers_post,$acceptLanguage_headers_post,$userAgent_headers_post,$contentType_headers_post,$accept_headers_post,$referer_headers_post,$xRequestedWith_headers_post,$connection_headers_post);
	
	
	
	
	//var data of post.
	$data_post;
	$id_data_post;
	$title_data_post;
	$update_data_postd;
	$subtitle_data_post;
	$type_data_post;
	$free_content_data_post;
	$content_data_post;
	$summary_data_post;
	$cover_data_post;
	$writer_data_post;
	$is_word_data_post;
	
	
	
	$id_data_post = $id_data_post;
	$text_data_post = $text_data_post;
	$follow_to_read_data_postd = '&follow_to_read=0';
	$follow_official_data_post = '&follow_official=0';
	$sync_wb_data_post = '&sync_wb=0';
	$is_original_data_post = '&is_original=0';
	$time_data_post = '&time=';
	
	
	$data_post = $id_data_post.$text_data_post.$follow_to_read_data_postd.$follow_official_data_post.$sync_wb_data_post.$is_original_data_post.$time_data_post;
	//含有data值的串联变量.
	
		/*
	 * 
	 * id=209124&text=%E5%8F%91%E5%B8%83%E4%BA%86%E5%A4%B4%E6%9D%A1%E6%96%87%E7%AB%A0%EF%BC%9A%E3%80%8A%E4%BD%A0%E5%8F%AA%E9%9C%80%E8%A6%81%E5%81%9A%E5%A5%BD%E4%BD%A0%E8%87%AA%E5%B7%B1%EF%BC%8C%E4%B8%80%E5%88%87%E9%83%BD%E6%98%AF%E5%89%AF%E4%BA%A7%E5%93%81test%E3%80%8B%20111&follow_to_read=0&follow_official=0&sync_wb=0&is_original=0&time=
	 */
	
	
	
	
	
	
	

	
	
	$url_post = 'https://card.weibo.com/article/v3/aj/editor/draft/publish';
	$curl = curl_init();
	curl_setopt($curl, CURLOPT_ENCODING, ""); //禁止curl数据压缩。
	curl_setopt($curl, CURLOPT_URL, $url_post);
	curl_setopt($curl, CURLOPT_POST, 1);
	//curl_setopt($curl, CURLOPT_HEADER, true);//禁止输出响应头
	curl_setopt ($curl, CURLOPT_HTTPHEADER , $headers_post);
	curl_setopt($curl, CURLOPT_POSTFIELDS, $data_post);
	curl_setopt ($curl, CURLOPT_RETURNTRANSFER, 1);//结果不直接输出到浏览器

	$result = curl_exec($curl);
	
	curl_close($curl);
	
	
	return $result;
	
	
}

function post_create_headarticle($cookies_global,$user_data_array_global)
{
	//函数功能：创造一个头条文章，服务器返回一个id
	
	//返回值：状态号码＋id
	
	
	$url_post;//Var url of post.
	$curl;//var curl.
	$user_data_array_global;
	
	$result;//var out.
	
	
	//Var header of post.
	$headers_post;
	$referer_headers_post;
	$userAgent_headers_post;
	$cookies_headers_post;
	$origin_headers_post;
	$acceptEncoding_headers_post;
	$acceptLanguage_headers_post;
	$contentType_headers_post;
	$accept_headers_post;
	$xRequestedWith_headers_post;
	$connection_headers_post;
	
	

	
	$url_post = 'https://card.weibo.com/article/v3/aj/editor/draft/create';
	$referer_headers_post = 'Referer: https://card.weibo.com/article/v3/editor';
	$userAgent_headers_post = 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/66.0.3359.170 Safari/537.36';
	$cookies_headers_post = $cookies_global;
	$origin_headers_post = 'Origin: https://card.weibo.com';
	$acceptEncoding_headers_post = 'Accept-Encoding: gzip, deflate, br';
	$acceptLanguage_headers_post = 'Accept-Language: zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7';
	$contentType_headers_post = 'Content-Type: application/x-www-form-urlencoded';
	$accept_headers_post = 'Accept: application/json, text/plain, */*';
	$xRequestedWith_headers_post = 'X-Requested-With: XMLHttpRequest';
	$connection_headers_post = 'Connection: keep-alive';

	
	//含有header值的数组
	$headers_post = array($cookies_headers_post,$origin_headers_post,$acceptEncoding_headers_post,$acceptLanguage_headers_post,$userAgent_headers_post,$contentType_headers_post,$accept_headers_post,$referer_headers_post,$xRequestedWith_headers_post,$connection_headers_post);
	
	
		//var data of post.
	$data_post;
	$title_data_post;
	$type_data_post;
	$summar_data_postd;
	$writer_data_post;
	$cover_data_post;
	$content_data_post;

	
	
	
	$title_data_post = 'title=%E6%9C%AA%E5%91%BD%E5%90%8D2';
	$type_data_post = '&type=draft';
	$summar_data_postd = '&summary=';
	$writer_data_post = '&writer=';
	$cover_data_post = '&cover=';
	$content_data_post = '&content=%3Cp%3E%E2%80%8B%3C%2Fp%3E';
	
	
	
	$data_post = $title_data_post.$type_data_post.$summar_data_postd.$writer_data_post.$cover_data_post.$content_data_post;
	//含有data值的串联变量.
	
		/*
	 * 
	 * title=%E6%9C%AA%E5%91%BD%E5%90%8D&type=draft&summary=&writer=&cover=&content=%3Cp%3E%E2%80%8B%3C%2Fp%3E
	 */
	
	
	
	
	
	
	
	$url_post = 'https://card.weibo.com/article/v3/aj/editor/draft/create';
	$curl = curl_init();
	curl_setopt($curl, CURLOPT_ENCODING, ""); //禁止curl数据压缩。
	curl_setopt($curl, CURLOPT_URL, $url_post);
	curl_setopt($curl, CURLOPT_POST, 1);
	//curl_setopt($curl, CURLOPT_HEADER, true);//禁止输出响应头
	curl_setopt ($curl, CURLOPT_HTTPHEADER , $headers_post);
	curl_setopt($curl, CURLOPT_RETURNTRANSFER, TRUE);
	curl_setopt($curl, CURLOPT_POSTFIELDS, $data_post);
	curl_setopt ($curl, CURLOPT_RETURNTRANSFER, 1);//结果不直接输出到浏览器
	

	$result = curl_exec($curl);
	//$result = curl_getinfo($curl,CURLINFO_CONTENT_TYPE); 
	curl_close($curl);
	
	
	return $result;
	
	
	
	
}

function post_upload_headarticle($cookies_global,$jpeg_data_post,$user_data_array_global)
{
	//函数功能：上传图片到微博头条文章
	//输入参数1:cookies
	//输入参数2:图片数据
	//输入参数3:用户数据
	
	//输出参数：上传图片后的html数据
	
		
	$url_post;//Var url of post.
	$curl;//var curl.
	$user_data_array_global;
	$result;//var out.
	
	
	
	//Var header of post.
	$headers_post;
	$referer_headers_post;
	$userAgent_headers_post;
	$cookies_headers_post;
	$origin_headers_post;
	$acceptEncoding_headers_post;
	$acceptLanguage_headers_post;
	$contentType_headers_post;
	$accept_headers_post;
	$xRequestedWith_headers_post;
	$connection_headers_post;
	
	$cacheControl_headers_post;
	$host_headers_post;
	$upgradeInsecureRequests_headers_post;

 
//Content-Length: 283883

 
	$url_post = 'https://picupload.weibo.com/interface/pic_upload.php?mime=image%2Fjpeg&marks=1&app=miniblog&s=rdxt&data=base64&url=0&markpos=1&logo=&nick=0&cb=https%3A%2F%2Fcard.weibo.com%2Farticle%2Fv3%2Fimageupload%3Fcallback%3DSTK_ijax_'.$user_data_array_global[15];
	$referer_headers_post = 'Referer: https://card.weibo.com/article/v3/editor';
	$userAgent_headers_post = 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/66.0.3359.170 Safari/537.36';
	$cookies_headers_post = $cookies_global;
	$origin_headers_post = 'Origin: https://card.weibo.com';
	$acceptEncoding_headers_post = 'Accept-Encoding: gzip, deflate, br';
	$acceptLanguage_headers_post = 'Accept-Language: zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7';
	$contentType_headers_post = 'Content-Type: application/x-www-form-urlencoded';
	$accept_headers_post = 'Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8';
	$xRequestedWith_headers_post = 'X-Requested-With: XMLHttpRequest';
	$connection_headers_post = 'Connection: keep-alive';

	$cacheControl_headers_post = 'Cache-Control: max-age=0';
	$host_headers_post = 'Host: picupload.weibo.com';
	$upgradeInsecureRequests_headers_post = 'Upgrade-Insecure-Requests: 1';
	
	//含有header值的数组
	$headers_post = array($cookies_headers_post,$origin_headers_post,$acceptEncoding_headers_post,$acceptLanguage_headers_post,$userAgent_headers_post,$contentType_headers_post,$accept_headers_post,$referer_headers_post,$xRequestedWith_headers_post,$connection_headers_post,$cacheControl_headers_post,$host_headers_post,$upgradeInsecureRequests_headers_post);
	
	
		//var data of post.
	$data_post;
	$jpeg_data_post;
	$base64_jpeg_data_post;
	$urlencode_base64_jpeg_data_post;

	$jpeg_data_post = file_get_contents($jpeg_data_post);// picture include
	$base64_jpeg_data_post = base64_encode($jpeg_data_post);//base64 encode of picture
	$urlencode_base64_jpeg_data_post = urlencode($base64_jpeg_data_post);//url encode of base64 of picture
	$data_post = 'b64_data='.$urlencode_base64_jpeg_data_post;
	
	
	

	
	
	$url_post = 'https://picupload.weibo.com/interface/pic_upload.php?mime=image%2Fjpeg&marks=1&app=miniblog&s=rdxt&data=base64&url=0&markpos=1&logo=&nick=0&cb=https%3A%2F%2Fcard.weibo.com%2Farticle%2Fv3%2Fimageupload%3Fcallback%3DSTK_ijax_'.$user_data_array_global[15];
	$curl = curl_init();
	curl_setopt($curl, CURLOPT_ENCODING, ""); //禁止curl数据压缩。
	curl_setopt($curl, CURLOPT_URL, $url_post);
	curl_setopt($curl, CURLOPT_POST, 1);
	curl_setopt($curl, CURLOPT_HEADER, true);//输出响应头
	curl_setopt ($curl, CURLOPT_HTTPHEADER , $headers_post);
	curl_setopt($curl, CURLOPT_RETURNTRANSFER, TRUE);
	curl_setopt($curl, CURLOPT_POSTFIELDS, $data_post);
	curl_setopt ($curl, CURLOPT_RETURNTRANSFER, 1);//结果不直接输出到浏览器
	//curl_setopt($curl, CURLOPT_FOLLOWLOCATION, 1);
	

	$result = curl_exec($curl);
	//$result = curl_getinfo($curl,CURLINFO_CONTENT_TYPE); 
	curl_close($curl);
	
	
	return $result;
	
	
	
	
	
}
function get_mid_tweet($source)
{
	//函数功能：获取帖子mid
	//输入参数1:html来源
	//输出参数：mid
	
	$source;
	$mid;
	$result;
	
	$source = $source;
	preg_match('/mid=\\\"([0-9]*)\\\"/i', $source,$mid);
	$result = $mid[1];
	
	return $result;
	
}

function get_pid_upload($source)
{
	//函数功能：获取上传图片的pid
	//输入参数1:html来源
	//输出参数：pid
	
	$source;
	$mid;
	$result;
	
	$source = $source;
	preg_match('/pid=([a-zA-Z0-9]*)/i', $source,$mid);
	$result = $mid[1];
	
	return $result;
	
}


function get_id_headarticle($source)
{
	//函数功能：获取创建头条文章的id
	//输入参数1:html来源
	//输出参数：id
	
	$source;
	$mid;
	$result;
	
	$source = $source;
	preg_match('/\"id\":\"([0-9]*)\"/i', $source,$mid);
	$result = $mid[1];
	
	return $result;
	
}



function test_get_singleContent($source)
{
	//method：用正则从批量文件，读取单个内容
	//parameters-1:html来源
	//return：数组
	
	$source;
	$singleContent;
	$result;

	$source = file_get_contents($source);
	preg_match_all('/[0-9]*、(.*)/i', $source,$singleContent);
	$result = $singleContent[1];
	
	return $result;
	
}

function batch_post_tweet($file)
{
	//method:读取批量文件，并发布到post
	//parameter-1:读取批量文件地址
	//return:当前条数
	
	$file=$file;
	$singleContent = test_get_singleContent($file);//读取外部函数，批量文件单条内容
	$result;
	$return;

foreach($singleContent as $value)//读取单条内容的数组，并且发送内容
{
	
	echo post_tweet($cookies_global,'&text='.$value,'&pic_id=',$user_data_array_global);//发布微博，无图片
	sleep(rand(60, 180));//参数为随机函数，防止发帖过于规律被发现
}

$result = '';
return $result;

}	






function post_tweet_picture($url_picture1,$url_picture2,$tweet)
{
	//method:发布含有2张图片的tweet
	//parametar-1:图片地址1
	//parametar-2:图片地址2
	//parametar-3:发布的内容
	//return:返回记录
	
	$url_picture1;
	$url_picture2;
	$tweet;
	$result;
	$return;
	
	$test_pid_1 = get_pid_upload(post_upload_tweet($cookies_global,$url_picture1,$user_data_array_global));

$test_pid_2 = get_pid_upload(post_upload_tweet($cookies_global,$url_picture2,$user_data_array_global));

$result = post_tweet($cookies_global,'&text='.$tweet,'&pic_id='.$test_pid_1.'|'.$test_pid_2,$user_data_array_global);//发布微博，无图片
	return $result;
	
}








function get_content($hostname,$username,$password,$database,$sql)
{
	//method:连接数据库
	//paramter1:目标数据库地址和端口
	//paramter2:用户名称
	//paramter3:密码
	//paramter4:指定数据库
	//paramter5:输入SQL语句
	//return:数据库句柄
	
	$hostname;//'localhost:3306'
	$username;//'root'
	$password;//''
	$database;
	$sql;
	$result;
	
	
	$database;
	$query;
	$results_database = mysqli_connect($hostname,$username,$password,$database);//需要选择数据库
	mysqli_set_charset($results_database,"utf8");//设置utf8编码
	$query = mysqli_query($results_database, $sql);//查询数据库
	$row = mysqli_fetch_all($query);//返回数据库的值
	
	$result = $row;
	mysqli_close($results_database); 
	
	return $result;
	
}


