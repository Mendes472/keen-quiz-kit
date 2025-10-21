# Quiz Master 🎯

A dynamic, interactive quiz game built with React, TypeScript, and Tailwind CSS. Test your knowledge across various topics including Geography, Science, History, Mathematics, Technology, Literature, and more!

## Features ✨

- **Dynamic Question Display**: One question at a time with smooth transitions
- **Multiple Choice Answers**: 4 options per question with instant feedback
- **Score Tracking**: Real-time score updates and progress indicator
- **Visual Feedback**: Color-coded correct/incorrect answers
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Beautiful UI**: Bold, vibrant colors with smooth animations
- **Share Results**: Share your score with friends

## How to Play 🎮

1. Click **"Start Quiz"** on the welcome screen
2. Read each question carefully
3. Select your answer from the four options (A, B, C, D)
4. Get instant feedback on your choice
5. The next question appears automatically after a short delay
6. View your final score and percentage at the end
7. Click **"Play Again"** to restart the quiz

## Technologies Used 🛠️

- **React 18** - UI framework
- **TypeScript** - Type safety
- **Vite** - Build tool and dev server
- **Tailwind CSS** - Styling
- **shadcn/ui** - UI components
- **Lucide React** - Icons
- **Sonner** - Toast notifications

## Installation & Setup 💻

```bash
# Clone the repository
git clone <repository-url>

# Navigate to project directory
cd quiz-master

# Install dependencies
npm install

# Start development server
npm run dev
```

The app will be available at `http://localhost:8080`

## Project Structure 📁

```
src/
├── components/
│   ├── Welcome.tsx          # Welcome/start screen
│   ├── Quiz.tsx             # Main quiz game logic
│   ├── QuestionCard.tsx     # Individual question display
│   ├── ProgressBar.tsx      # Progress and score indicator
│   └── Results.tsx          # Final results screen
├── data/
│   └── questions.ts         # Question bank
├── pages/
│   └── Index.tsx            # Main page with game state
└── ...
```

## Customization 🎨

### Adding New Questions

Edit `src/data/questions.ts` to add new questions:

```typescript
{
  id: 11,
  question: "Your question here?",
  options: ["Option A", "Option B", "Option C", "Option D"],
  correctAnswer: 0, // Index of correct answer (0-3)
  category: "Category Name"
}
```

### Changing Colors

The design system is defined in `src/index.css`. Modify CSS variables to change the color scheme:

```css
:root {
  --primary: 245 60% 55%;      /* Main theme color */
  --success: 145 65% 45%;      /* Correct answers */
  --destructive: 355 75% 55%;  /* Incorrect answers */
  /* ... more colors */
}
```

## Future Enhancements 🚀

Potential features to add:
- Timer for each question
- Multiple quiz categories/difficulty levels
- Leaderboard with high scores
- User accounts and progress tracking
- API integration for dynamic questions
- Sound effects and music
- Multiplayer mode
- Question explanations

## Error Handling 🛡️

The application includes:
- TypeScript type safety to prevent runtime errors
- Graceful handling of invalid data
- Responsive error states
- Toast notifications for user feedback

## Contributing 🤝

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License 📄

This project is open source and available under the MIT License.

## Acknowledgments 🙏

- Built with [Lovable](https://lovable.dev)
- UI components from [shadcn/ui](https://ui.shadcn.com)
- Icons from [Lucide](https://lucide.dev)

---

Made with ❤️ using React and TypeScript
