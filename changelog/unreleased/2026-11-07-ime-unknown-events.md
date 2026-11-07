- **Rune builds against winit forks that add IME events.** A window matched every
  `winit::event::Ime` variant, so a winit fork with another one (such as an
  `Ime::DeleteSurrounding` for surrounding-text deletion) failed to compile Rune. Events Rune does
  not take yet are now ignored.
