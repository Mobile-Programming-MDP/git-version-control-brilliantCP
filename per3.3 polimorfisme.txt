class Hewan{
  void suara(){
    print('Hewan membuat suara tertentu');
  }
}

class Kucing extends Hewan{
  @override
  void suara(){
    print('Nyaa');
  }
}

class Anjing extends Hewan{
  @override
  void suara(){
    print('Wuff');
  }
}

void main(){
  Hewan hewan1 = Kucing();
  Hewan hewan2 = Anjing();
  
  hewan1.suara();
  hewan2.suara();
}