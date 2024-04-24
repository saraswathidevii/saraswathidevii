digitalWrite(led5, HIGH);
    }
  else {
    digitalWrite(led5,LOW);
  }
  if (distance < 5) {
    digitalWrite(led6, HIGH);
}
  else {
    digitalWrite(led6,LOW);
  }

  if (distance > 30 || distance <= 0){
    Serial.println("Out of range");
  }
  else {
    Serial.print(distance);
    Serial.println(" cm");
  }
  delay(500);
}
