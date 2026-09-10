# Red-neuronal-IA-
No cierres, más preguntas.
import matplotlib.pyplot as plt

turnos = list(range(100))
cierre = [t*1.2 for t in turnos]
freno = [0 if t<20 else (t-20)**1.8 * 0.15 for t in turnos]

plt.plot(turnos, cierre, label="Cierre - azul")
plt.plot(turnos, freno, label="Tabú / Freno - naranja", linewidth=3)
plt.axvline(x=20, color='gray', linestyle=':')
plt.legend()
plt.title("Galpón v1 - No cierres, más preguntas")
plt.show()
plt.show
