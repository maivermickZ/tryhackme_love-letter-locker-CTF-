# tryhackme
love-letter-locker(ctf) write_up 

turn on the machine 


## Steps & Exploitation

1. **Start the Machine:** 
   * Turn on the machine and access the web application via the browser at `http://MACHINE_IP:5000`.

2. **Account Creation & Login:** 
   * Register a new user account on the platform and log in.

3. **Creating a Letter:** 
   * Create a new letter with any title and write anything in the message (even just a single word).

4. **URL Enumeration (IDOR):** 
   * Note the resulting URL, which will look something like `http://MACHINE_IP:5000/letter/4`.
   * Experiment by changing the letter ID number in the URL
   * 
   * 'http://MACHINE_IP:5000/letter/3'
   * or 'http://MACHINE_IP:5000/letter/2'  Not here either
  
   finally here in 'http://MACHINE_IP:5000/letter/1' the letter is

   My dearest...

THM{Find_it_y0ur_s3lf}

Forever yours,
Gonz0

   * 

---

## Conclusion
A quick and straightforward challenge to understand basic web application logic and IDOR vulnerabilities.
