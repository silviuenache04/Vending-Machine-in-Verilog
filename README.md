Design an FSM for an automatic chocolate selling machine, which delivers chocolates at 2.5€. The machine accepts only coins of 50 cents and 1 euro, and does not return any change. When the amount of 2.5€ or more is reached, the machine delivers a chocolate and will resume the process, subtracting 2.5€ from the current amount. The process resumes with whatever amount remains after delivering, which may be 0 or 0.5€.

The inputs are the digital signals cents, euro and ack.

When the user inserts a valid coin, the corresponding input, cents or euro, is asserted and stays 1 for some clock cycles. The FSM considers the coin validated only after the corresponding input goes back to 0.

The output is a digital signal, deliver, that is asserted when the amount reaches or surpasses 2.5€ and stays asserted until the input ack is asserted. The FSM resumes the process after ack is deasserted.
