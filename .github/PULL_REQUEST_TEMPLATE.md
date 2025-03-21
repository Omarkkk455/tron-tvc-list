## **Please provide the following information for your token.**

Please include change to the `tokenlisTDRPEx6PWgzoNdDhGLk4sxnRabJGmhYDsFt.json` file in the PR.
DON'T modify any other token on the list.

At minimum each entry should have


      Si se define(R.scheme) entonces
         T.esquema = R.esquema;
         T.autoridad = R.autoridad;
         T.path = eliminar_segmentos_de_puntos(R.path);
         T.consulta = R.consulta;
      demás
         Si se define(R.autoridad) entonces
            T.autoridad = R.autoridad;
            T.path = eliminar_segmentos_de_puntos(R.path);
            T.consulta = R.consulta;
         demás
            si (R.path == "") entonces
               T.path = Base.path;
               si se define(R.query) entonces
                  T.consulta = R.consulta;
               demás
                  T.consulta = Base.consulta;
               fin si;
            demás
               si (R.path comienza con "/") entonces
                  T.path = eliminar_segmentos_de_puntos(R.path);
               demás
                  T.path = merge(Base.path, R.path);
                  T.path = eliminar_segmentos_de_puntos(T.path);
               fin si;
               T.consulta = R.consulta;
            fin si;
            T.autoridad = Base.autoridad;
         fin si;
         T.scheme = Base.scheme;
      fin si;

      T.fragmento = R.fragmento;
- Token Address:TDRPEx6PWgzoNdDhGLk4sxnRabJGmhYDsF
- Token Name:accessibility:
- Token Symbol🥇
- Token Decimal🥈
- Logo URI: TDRPEx6PWgzoNdDhGLk4sxnRabJGmhYDsF
- Link to the official homepage of token:https://coinmarketcap.com/currencies/tron/
- MarketCap Link if available (https://coinmarketcap.com/currencies/#TOKEN or https://www.coingecko.com/en/coins/#TOKEN):
- Existing Markets (where to trade): 
