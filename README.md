
# Rapport

Det som jag har gjort i denna uppgift är 3 widgets som kommer up på home screen och tänkte gå igenom dom 1 och 1

Först gjode jag en textview med syftet att den ska vara en välkommst till appen
Koden ser ut såhär:
```
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Välkommen till JanneAppen!"
        android:id="@+id/janne_label"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

Detta ska vara pappan till allt och jag har ändrat vart dom andra widgetsen ska ligga från denna textview. Har inte ändrat så mycket förutom att jag gav den ett id

Knappens ska ligga under textviewen och ska vara som en login knapp. såklart funkar den inte eftersom jag inte har nån onClick() i koden. För att den skulle ligga under textviewen gjorde jag såhär:

    <Button
        android:layout_width="100dp"
        android:layout_height="40dp"
        android:text="Logga in"
        android:id="@+id/signin"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toBottomOf="@id/janne_label" />

Längst ner kan man se att layout_constraintTop_toBottomOf har textviewens id. Då kommer den att lägga sig strax under textviewen

Ungefär samma sak gjorde jag på editviewen också:
<EditText
        android:layout_width="300dp"
        android:layout_height="wrap_content"
        android:text="Vad har du gjort idag?"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toBottomOf="@id/signin"
    />

Gav den en text som den ska börja med att skriva ut så att användaren ska förstå vad den ska skriva. Sen kan man se att id som jag gav till min knapp nu ligger längst ner här så att denna text lägger sig under knappen
Jag skulle säga att man kan se detta som en hierarki



