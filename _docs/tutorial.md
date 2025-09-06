\# Tutorial







from PyCliffordMCP import Circuit, Measurement



\# Create a 2-qubit circuit

c = Circuit(2)



\# Apply gates

c.h(0)   # Hadamard on qubit 0

c.cx(0,1) # CNOT from qubit 0 to 1



\# Measure

m = Measurement(c)

result = m.run()

print(result)





