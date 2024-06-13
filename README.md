python
  try:
      raise ExceptionGroup("group", [ValueError("error1"), TypeError("error2")])
  except* ValueError as e:
      print(f"Caught ValueError: {e}")
  except* TypeError as e:
      print(f"Caught TypeError: {e}")
  