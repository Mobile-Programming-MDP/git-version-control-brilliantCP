class Mahasiswa{
  String _nama;
  int _umur;
  
  Mahasiswa(this._nama, this._umur);
  
  String get nama => _nama;
  
  set nama(String value){
    if(value.isNotEmpty){
      _nama = value;
    }
  }
  
  int get umur => _umur;
  
  set umur(int value){
    if(value >= 17 && value <= 40){
      _umur = value;
    }
  }
}

void main(){
  var mahasiswa = Mahasiswa('John', 20);
  
  print('Nama Mahasiswa: ${mahasiswa.nama}');
  print('Umur Mahasiswa: ${mahasiswa.umur}');
  
  mahasiswa.nama = 'Jane';
  mahasiswa.umur = 22;
  
  print('Nama Mahasiswa: ${mahasiswa.nama}');
  print('Umur Mahasiswa: ${mahasiswa.umur} tahun');
}