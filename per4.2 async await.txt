void main() async{
  print("Getting your order....");
  var order = await getOrder();
  try{
    print("Your Order : $order");    
  }catch(error){
    print("Sorry, $error");
  }finally{
    print("Thank You");
  }

}

Future<String> getOrder(){
  return Future.delayed(Duration(seconds: 3), (){
    var isStockAvailable = false;
    if(isStockAvailable){
      return "Coffee Boba";
    }else{
      throw "Out of Stock";
    }
      
  });
}