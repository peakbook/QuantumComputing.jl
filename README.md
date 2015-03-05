## QuantumComputing.jl

Julia package for quantum computing.

### Example

```julia
using QuantumComputing

psi = Ket(0,0,0,0)
n = length(psi)

println("input:")
println(psi)

psi = Hadamard(n,4)*GCNot(n,1,2,3)*Not(n,3)*Not(n,2)*psi

println("output:")
println(psi)
```

```
input:
1.0000000000000	|0000⟩ 

output:
0.5000000000000	|1110⟩ 
0.5000000000000	|1111⟩ 

```
