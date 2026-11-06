
cat > .gitignore <<'EOF'
.env
.env.*
!.env.example
.aws/
*.pem
*.key
*.log
__pycache__/
.DS_Store
EOF

