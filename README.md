
# Rapport

**Skriv din rapport här!**

_Du kan ta bort all text som finns sedan tidigare_.

## Följande grundsyn gäller dugga-svar:


1. Adderade mountain names i array
2. Jag skapade en loop för att recycleview ska fungera
3. adderade Json url och json file 
4. skapade en post execute så att Json så att Json fungerar och google adderade jag som import för att få den att fungera
5. adderad wifi också
```
 items.add(new Mountain("Berf"));
        items.add(new Mountain("Neft"));
        items.add(new Mountain("Gurt"));
        
        
           for (int i =0;i<items.size();i++) {
            Log.d("Vinge", "" + items.get(i).toString());
            recyclerViewItems.add(new RecyclerViewItem(items.get(i).toString()));
        }
        
        import androidx.annotation.NonNull;
        
        
    private final String JSON_URL = "HTTPS_URL_TO_JSON_DATA_CHANGE_THIS_URL";
    private final String JSON_FILE = "mountains.json";
    
    
     public void onPostExecute(String json) {
        Log.d("MainActivity","" + json);

        Type type = new TypeToken<List<Mountain>>() {}.getType();
items = gson.fromJson(json, type);
for (Mountain m : items) {
    recyclerViewItems.add(new RecyclerViewItem(m.getName()));
    
     <uses-permission android:name="android.permission.INTERNET" />

```

Bilder läggs i samma mapp som markdown-filen.

![](Screenshot_20240503_095120.png)

Läs gärna:

- Boulos, M.N.K., Warren, J., Gong, J. & Yue, P. (2010) Web GIS in practice VIII: HTML5 and the canvas element for interactive online mapping. International journal of health geographics 9, 14. Shin, Y. &
- Wunsche, B.C. (2013) A smartphone-based golf simulation exercise game for supporting arthritis patients. 2013 28th International Conference of Image and Vision Computing New Zealand (IVCNZ), IEEE, pp. 459–464.
- Wohlin, C., Runeson, P., Höst, M., Ohlsson, M.C., Regnell, B., Wesslén, A. (2012) Experimentation in Software Engineering, Berlin, Heidelberg: Springer Berlin Heidelberg.
