# Vulcano con eruzione di particles
Abbiamo deciso che per il nostro progetto faremo un vulcano che erutta particles usando una camera ortografica
# Aggiunto vulcano
Il vulcano aggiunto è stato fatto su MagicaVoxel. Mancano però le texture in quanto è stato esportato in .obj e non è stato immediato capire come sfruttare il file .mtl e .png per le texture
# Aggiunta libreria MTLLoader
Le texture sono state aggiunte usando la libreria MTLLoader, che è stata aggiunta ed è stata implementata in una funzione.
# Modifica luci
Modificate le luci per ottenere un effetto più drammatico
# Aggiunta particles ShaderParticleEngine
Sono state aggiunte le particles sfruttando la libreria ShaderParticleEngine (SPE). 
# Posizionate le particles
Sono state posizionate le particles perché eruttassero dal cratere. C'è però un problema: non è possibile ruotare la camera con gli OrbitControls.
# Sistemato problema OrbitControls
Dopo una lunga indagine, è stato realizzato che le particles fossero buggate a causa di questo listener: controls.addEventListener('change', Render);. Una volta rimpiazzato con una diversa istanziazione di controls, il problema della rotazione della camera con le particles è stato risolto.
# Aggiornato progetto in modo che funzionasse con Heightmap
Il progetto è stato aggiornato per funzionare con una Heightmap del vesuvio.