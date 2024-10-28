# OriginTrail-DKG-V8-incentivised-testnet

![EDge](https://github.com/user-attachments/assets/c4bcbf2e-16c3-4712-a697-22ff2560366d)


[Twitter](https://x.com/origin_trail/status/1849493586083029052) \
[Discord](https://discord.gg/cys86MB8GE) \
[Website](https://origintrail.io/) \
[Dashboard](https://dkg-v8-incentivised-testnet.origintrail.io/)

### Spek Run Node
- Ubuntu 20 atau 22
- CPU 2 Core
- Ram 4
- Storage 50 Gb
- Open Port ( 8900, 9000 )

### Step Run Node by Maouam Node Labs
1. Buat dua wallet di metamask (simpan utk kebutuhan instalasi) 
   - wallet pertama operasional (simpan private key dan address) 
   - wallet kedua untuk admin (simpan address) 


2. Isi Wallet Pertama dengan Eth Base Sepolia \
   Atau bisa bridge di orbiter sepolia ke base sepolia \
   [Link Bridge Orbiter](https://rinkeby.orbiter.finance/?source=Sepolia&dest=BaseSepolia&token=ETH) 


3. Claim faucet TRAC di discord `channel faucet-bot` \
   [Faucet Discord Link](https://discord.gg/cys86MB8GE)


4. Install dan run node
   ```
   cd /root/ && curl -k -o v8_installer.sh https://raw.githubusercontent.com/OriginTrail/ot-node/v8/develop/installer/v8_installer.sh && chmod +x v8_installer.sh
   ./v8_installer.sh
   ```

5. Setelah Install Selesai akan ada pilihan Ikuti instruksi
  - Please select the database you would like to use: (Default: Blazegraph) [1]Blazegraph [2]Fuseki [E]xit: 
    ```
    (PILIH 1, ENTER)
    ```
  - Please select the SQL you would like to use: (Default: MySQL) [1]MySQL [2]MariaDB [E]xit 
    ```
    (PILIH 1, ENTER)
    ```
  - Would you like to change your sql password or add one ? (Default: Yes) [Y]es [N]o [E]xit 
    ```
    (Y lalu ENTER)
    ```
  - Enter your new sql password: 
    ```
    (BUAT PASSWORD BARU UNTUK DATABASE)
    ```
  - Please confirm your new sql password: 
    ```
    (ULANG KETIK PASSWORD UNTUK DATABASE)
    ```
  - Please insert your operational wallet public key no. 1: 
    ```
    (PASTE ADDRESS WALLET PERTAMA)
    ```
  - Please insert private key for your operational wallet no. 1:
    ```
    (PASTE PRIVATE KEY WALLET PERTAMA)
    ```
  - Please insert your operational wallet public key no. 2:
    ```
    (ENTER, UNTUK SKIP, IKUTIN AJA YG GUA BLG YAAKKK)
    ```
  - Enter your EVM management wallet address :
    ```
    (PASTE ADDRESS WALLET KEDUA)
    ```
  - Enter your profile shares token name :
    ```
    (BEBAS MAU NAMA APA AJA, MAU DI BUAT KUCING ATAU ASU BEBASSS)
    ```
  - Enter your profile shares token symbol :
    ```
    (SAMAIN AJA SAMA NAMA TOKEN NAME)
    ```
  - Enter your operator fee for Base Sepolia (0-100):
    ```
    (5 sampai 10 aja, jgn banyak2, tapi terserah lu kalau mau 100)
    ```
  - Enter your RPC endpoint:
    ```
    https://base-sepolia-rpc.publicnode.com
    ```

6. Kalau udah ada log kyk tulisan V8 atau Operation ID, berarti instalasi sukses, boleh `ctrl c` yak utk stop log 
7. Untuk Cek logs `(stop logs ctrl c)`
   ```
   journalctl -u otnode --output cat -fn 100
   ```
8. Cek status node `(active/running atau sedang stop)`
   ```
   Cek status node (active/running atau sedang stop)
   ```
9. Cek Dashboard \
   https://dkg-v8-incentivised-testnet.origintrail.io/ 


### DONE
