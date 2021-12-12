## Feedback

Task 2 looks good. On your query you could have just said "SELECT DISTINCT card_no FROM `umt-msba.transactions.transArchive*`". 

Task 3 looks good as well. I'd be curious if you could change `cursor.execute(f"INSERT INTO salesbyhour VALUES('{Date}','{Hour}','{Total_spend}','{Transactions}','{Items}')")`
to something like `cursor.execute(f"INSERT INTO salesbyhour VALUES('{row[0]}','{row[1]}','{row[2]}','{row[3]}','{row[4]}')")`. Might have been 
a bit simpler. That goes for everything else as well. At any rate, this all looks correct, so you can cross these two pieces off your list. 
