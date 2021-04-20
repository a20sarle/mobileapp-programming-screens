
# Rapport för uppgift 3: Screens

Den andra aktiviteten lades till genom att skapa filen LoginActivity.java som medförde filen activity_login.xml . En lade i och med detta också till koden nedan i AndroidManifest.xml för att säga till vilken aktivitet som skulle köras och i vilken ordning.
```
<activity android:name=".LoginActivity">
    <intent-filter>
        <action android:name="android.intent.action.MAIN" />

        <category android:name="android.intent.category.LAUNCHER" />
    </intent-filter>
</activity>
```
Den andra sidan skulle inte visa vidare till någon ny _screen_ och _intent_ togs därav bort från aktiviteten kallad MainActivity.


För att skapa knappen på första _screen_ bytten en ut TextView i activity_login.xml mot Button och därefter gick en till LoginActivity.java och importerade tre bibliotek för att kunna lägga till och testa knappfunktionen.
```
Button buttonLogin = findViewById(R.id.button_login);
buttonLogin.setOnClickListener(new View.OnClickListener() {
    @Override
    public void onClick(View v) {
        Log.d("TAG","Hej!");
    }
});
```
```
import android.util.Log;
import android.view.View;
import android.widget.Button;
```


För att göra så att en kunde gå vidare till _screen_ nummer två behövdes en _intent_ skapas på sidan LoginActivity.java. Genom intent sägs att en befinner sig på LoginActivity och sedan ska gå till MainActivity. Även här behövdes ett bibliotek importeras.
```
import androidx.appcompat.app.AppCompatActivity;
```
```
Intent intent = new Intent(LoginActivity.this,MainActivity.class);
startActivity(intent);
```


_Fragmentet_ skapades







```
f
```


![](android.png)
