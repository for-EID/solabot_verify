## solabot verify via Ledger Hardware Wallet

how to connect your Solana address to your Discord account via solabot and Ledger  

join us at [Discord](https://discord.gg/watWTScK)  


[verify channel](#verify-channel)  
[allow solabot](#allow-solabot)  
[choose Ledger](#choose-ledger)  
[verification Transaction](#verification-transaction)  
[get Tx to verify](#get-tx-to-verify)  
[get Tx URL](#get-tx-url)  
[fill Tx URL in solabot form](#fill-tx-url-in-solabot-form)  
[check your discord role](#check-your-discord-role)  

**[KNOWN ISSUES](#known-issues)**  
[cant choose Ledger on SolaBots website](#cant-choose-ledger-on-solabots-website)  
[cant verify transaction](#cant-verify-transaction)  

---

### verify channel  

jump to your Discord verify channel (1) and click on the link (2)  

![discord_verify_channel](pic/1_discord_verify_channel.png)  


### allow solabot  

authorize bot to access your username    

![allow_solabot](pic/2_allow_solabot.png)  


### choose Ledger  

on the solabot website choose "Other / Ledger"  

![choose_ledger](pic/3_solabot_website_choose_ledger.png)  


### verification Transaction  

the solana app on Ledger can't sign messages at the moment. because of this you have to verify your ownership via a transaction  

in this example we use phantom wallet which is connected to our Ledger to do the transaction  
(1) enter the exact amount shown on the website to your transaction (send SOL - nothing else)  
(2) copy your own Solana address  
(3) paste your address and send the amount  

![send_sol](pic/4_send_sol_phantom.png)  

**if you don't have this two buttons go to [known issues](#known-issues)**  

### get Tx to verify  

(1) select transaction history in phantom  
(2) klick on the transaction where you sent the amount from last step  

![phantom_get_tx](pic/5_phantom_get_tx.png)  


### get Tx URL

copy the URL from your browser

![copy_url](pic/6_get_tx_url.png)  


### fill Tx URL in solabot form  

paste the URL you got in last step to the form on solabot website  

![fill_tx_form](pic/6_fill_tx_link_solabot.png)  


### check your discord role  

follow all other steps in the discord verify channel  
the bot checks the wallets every hour. after a while check your roles in discord.  

![check_discord_role](pic/7_discord_check_role.png)   

---

## KNOWN ISSUES  

### cant choose Ledger on SolaBots website  

you can't select "Other / Ledger" on solabot website  

go to your user settings in your Discord app  
jump to "Authorized Apps"  
Deauthorize SolaBots  

![deauthorize_solabot](pic/8_remove_solabot_from_discord.png)  

remove the site access to your wallet  

open phantom and go to settings - "Trusted Apps"  

![remove_phantom_site_access](pic/9_remove_solabot_from_phantom.png)  

revoke site access to your wallet  

![revoke_access_in_phantom](pic/10_remove_solabot_from_phantom2.png)

continue with [verify channel](#verify-channel)    

**HINT:** if this still don't work copy the solabot site URL and use a different browser - preferably one without a solana wallet plugin  

continue with [choose Ledger](#choose-ledger)  


### cant verify transaction  

check if the mint of the NFTs is still ongoing. In this case the json is not updated and the verification will not work.  
Wait for the mint to finish and try again to verify your transaction.  

---
