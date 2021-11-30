# cek-rumah
#include <iostream>
using namespace std;
int main(){
	int n;
	bool status = false;
	cout<<"Banyaknya Rumah Griya Asri: ";
	cin>>n;
	string namaCek;
	string alamatCek;
	string nama[n];
	string alamat[n];
    for(int i=0;i<n;i++){
		cout<<"Masukkan nama pemilik rumah: ";
		cin>>nama[i];
		cout<<"Masukkan alamat rumah: ";
		cin>>alamat[i];

	}
	cout<<"Masukkan nama pemilik rumah yang ingin dicek: ";
	cin>>namaCek;
	cout << "Masukkan alamat pemilik rumah yang ingin dicek: ";
	cin>>alamatCek;
	cout<<endl;
	cout<<endl;
	for(int i=0;i<n;i++){
		if(namaCek==nama[i]&&alamatCek==alamat[i]){
			status=true;
			cout<<"Rumah ditemukan"<<endl;
			break;
		}
	}
	if(status==false){
		cout<<"Rumah tidak ditemukan";
	}

}
