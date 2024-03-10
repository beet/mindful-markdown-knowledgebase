## ✅ Today

```tasks
(due today) OR (scheduled today)
not done
path regex does not match /Weekly [Rr]eview \d{4}-\d{2}-\d{2}/
```

```tasks
done on today
```

## Yesterday

```tasks
(due yesterday) OR (scheduled yesterday)
filename regex does not match /Weekly review [\d]{4}-[\d]{2}-[\d]{2}/
not done
```

```tasks
done yesterday
```

## 🔴 Overdue

```tasks
not done
(due before yesterday) OR (scheduled before yesterday)
filename regex does not match /Weekly review [\d]{4}-[\d]{2}-[\d]{2}/
status.name regex does not match /progress|cancelled|forwarded|scheduling|question|important|star|quote|location|bookmark|info|savings|idea|pros|cons|fire|key|win|up|down/
```

## 🗓 This week

```tasks
not done
(due after today) OR (scheduled after today)
(due before this saturday) OR (scheduled before this saturday)
```
