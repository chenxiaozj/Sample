##Samples

###Connectivity
1. BasicNetworking
	* 日志输出到多个target中，demo在原生日志的基础上还将日志输出到了页面的textview上，demo中每一个LogNode即是一个target，可以通过setNext方法设置输出到不同的target上
	* 判断网络连接的方式：wifi，数据业务
2. NetworkConnect

     	URL url = new URL(urlString);
        HttpURLConnection conn = (HttpURLConnection) url.openConnection();
        conn.setReadTimeout(10000 /* milliseconds */);
        conn.setConnectTimeout(15000 /* milliseconds */);
        conn.setRequestMethod("GET");
        conn.setDoInput(true);
        // Start the query
        conn.connect();
        InputStream stream = conn.getInputStream();
        
 3. BasicAndroidKeystore
 	* 主要介绍非对称加密，生成keypair，给私钥签名加密以及校验，更详细的demo参见<http://blog.csdn.net/wangqiuyun/article/details/42143957>