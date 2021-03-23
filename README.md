# ex_hoso
# network

cd network
sudo ./byfn down && docker ps -aq && docker images dev-* -q

# server
cd ../server
sudo ./startFabric.sh

## javascript
cd javascript
rm -rf wallet && node enrollAdmin.js && node registerUser.js && node apiserver.js

# test
## getall
http://127.0.0.1:5000/api/queryallbn

## getone
http://127.0.0.1:5000/api/query/BN1

## post
http://127.0.0.1:5000/api/addbn

{
    "bnid": "BN12",
    "mabn": "2020083148",
    "hoten": "Nguyễn Thị Hồng Hoa",
    "ngaysinh": "28/08/1955",
    "gioitinh": "Nữ",
    "cmnd": "abc",
    "diachi": "80/28 PNL, Phường An Hòa, Quận Ninh Kiều, Thành phố Cần Thơ",
    "maxa": "9291831177"
}

