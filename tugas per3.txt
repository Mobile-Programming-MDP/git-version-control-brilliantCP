class PersegiPanjang{
  double panjang;
  double lebar;
  
  PersegiPanjang(this.panjang, this.lebar);
  
  double hitungLuas(){
    return panjang * lebar;
  }
  double hitungKeliling(){
    return 2 * (panjang + lebar);
  }
  
}

void main(){
  double panjang = 5;
  double lebar = 3;
  
  var persegiPanjang = PersegiPanjang(panjang, lebar);
  var luasPersegiPanjang = persegiPanjang.hitungLuas();
  var kelilingPersegiPanjang = persegiPanjang.hitungKeliling();
  
  print("Luas Persegi : $luasPersegiPanjang");
  print("Keliling Persegi : $kelilingPersegiPanjang");
}