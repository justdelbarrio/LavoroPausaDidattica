# CassaforteMain

Properties:

        // Numero di matricola della cassaforte
        public int NumeroMatricola { get; set; }

        // Produttore della cassaforte
        public string Produttore { get; set; }

        // Modello della cassaforte
        public string Modello { get; set; }

        // Codice di sblocco segreto della cassaforte
        private string CodiceSblocco { get; set; }

        // Codice utente impostato per aprire la cassaforte
        private string CodiceUtente { get; set; }

        // Data per l'apertura programmata della cassaforte
        private DateTime DataProgrammata { get; set; }

        // Conteggio delle aperture effettuate con successo dalla creazione della cassaforte
        public int ApertureEffettuate { get; set; }

        // Conteggio delle aperture tentate dalla creazione della cassaforte
        public int ApertureTentate { get; set; }

        // Var per verificare se la cassaforte è bloccata
        private bool Bloccata { get; set; }

        // Var per verificare lo stato di apertura 
        private bool Stato { get; set; }

        // Data corrente
        public DateTime DataCorrente { get; set; }

        // Numero di tentativi di apertura di fila falliti
        public int TentativiFalliti { get; set; }
        
Funzioni:

         - Costruttore base
         - public void ImpostaCodiceUtente(string codiceUtente)  // Imposta il codice utente per aprire la cassaforte
         - public void Apri(string codiceUtente)  // Apre la cassaforte se il codice utente corrisponde a quello impostato
         - public void Chiudi() // Chiude la cassaforte
         - public void Sblocca(string codiceSblocco) //Sblocca la cassaforte
         - public void GeneraCod(string codiceUtente) //Genera un codice casuale a 5 cifre
         - public void ImpostaData(DateTime data) //Imposta la data all'attributo DataProgrammata
         - public bool AperturaProgrammata(string codiceUtente) // Metodo per aprire la cassaforte
         - public Cassaforte Clone() //Metodo per clonare una variabile di tipo Cassaforte
         -  public string ToString() //Metodo che prende tutti gli attributi e gli unisce in una sola stringa
        
        
