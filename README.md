# Base64Encoder-for-iOS
Convert Data Image to Base64 String on iOS

Usage on Swift 2.0

  let theImage : UIImage = UIImage(named:"image-name")
  var imageData = UIImageJPEGRepresentation(theImage, 1)
  var base64String = Base64Convertor.encodeBase64WithData(imageData)
  print("\(base64String)")


    +(NSString *)encodeBase64WithString:(NSString *)strData ;

    +(NSString *)encodeBase64WithData:(NSData *)objData;

    +(NSData *)base64DataFromString: (NSString *)string;
