User (Browser)
      ↓
Frontend — React + TypeScript (Vercel pe deploy)
      ↓
Backend — Python + FastAPI (Render pe deploy)
      ↓
External API — Copernicus CDS (ERA5 weather data)


HydroAlert/
├── flood_model/
│   ├── api_server.py        ← FastAPI server
│   ├── flood_predictor.py   ← Core risk engine
│   ├── flood_with_ollama.py ← AI explanation
│   ├── finetune_model.py    ← Model tuning
│   ├── flood_data.nc        ← Sample data
│   └── *.grib / *.idx       ← ERA5 data files
├── frontend/
│   ├── src/
│   │   ├── components/      ← React components
│   │   ├── services/api.ts  ← Backend connection
│   │   └── App.tsx          ← Main app
│   └── package.json
└── requirements.txt         ← Python dependencies
