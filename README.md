# bryt_gmng
START
    DECLARE balance, rate, interest, newBalance AS REAL

    PROMPT "Enter account balance: "
    READ balance

    IF balance >= 10000 THEN
        rate = 0.05
    ELSE
        rate = 0.02
    ENDIF

    interest = balance * rate
    newBalance = balance + interest

    PRINT "Interest earned = ", interest
    PRINT "New balance = ", newBalance
STOP
